### Search for a contraint
```
select * from all_constraints
where constraint_name = 'SYS_C00475824'
/
```

### Extend password expiration date
```
select * from dba_profiles;

ALTER PROFILE DEFAULT LIMIT PASSWORD_LIFE_TIME UNLIMITED;

 select 'alter user "'||d.username||'" identified by values '''||u.password||''';' c
from dba_users d, sys.user$ u
where d.username = upper('&&username')
and u.user# = d.user_id;   

alter user "EDNADB" identified by values 'BC9EA855F06FEC11';

commit;
```

### Generate random values between 1-99
```
select ROUND(DBMS_Random.Value(1,99)) from Dual
```

