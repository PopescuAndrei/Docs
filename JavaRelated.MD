@PreAuthorize("hasRole('ROLE_XYZ')") is the same as @PreAuthorize("hasAuthority('ROLE_XYZ')") and in Spring security 4 
@PreAuthorize("hasRole('XYZ')") is the same as @PreAuthorize("hasAuthority('ROLE_XYZ')").

For MariaDB, the connection properties look like this:

```java
'db.dialect' : 'org.hibernate.dialect.MariaDB53Dialect',
'jdbc.driver': 'org.mariadb.jdbc.Driver',
'jdbc.user' : 'hibernate_orm_test',
'jdbc.pass' : 'hibernate_orm_test',
'jdbc.url' : 'jdbc:mariadb://127.0.0.1/hibernate_orm_test'
```
While the URL includes the mariadb database identifier, the MariaDB53Dialect supports Time and Timestamp with microsecond precision, just like MySQL57InnoDBDialect.
