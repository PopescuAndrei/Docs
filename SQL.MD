### Search for a contraint
```sql
select * from all_constraints
where constraint_name = 'SYS_C00475824'
```

### Extend password expiration date
```sql
select * from dba_profiles;

ALTER PROFILE DEFAULT LIMIT PASSWORD_LIFE_TIME UNLIMITED;

 select 'alter user "'||d.username||'" identified by values '''||u.password||''';' c
from dba_users d, sys.user$ u
where d.username = upper('&&username')
and u.user# = d.user_id;   

alter user "USERNAME" identified by values 'THE_HASH_FROM_THE_LAST_STATEMENT_RESULT';

commit;
```

### Generate random values between 1-99
```sql
select ROUND(DBMS_Random.Value(1,99)) from Dual
```

### Copy entire table and records in another table
```sql
CREATE TABLE dbtable_copy
	AS (SELECT * FROM dbtable);
 ```
