

\d[S+] [ pattern ]

\d tablename
\d+ tablename





\d
```
postgres=# \d
        List of relations
 Schema |  Name   | Type  | Owner
--------+---------+-------+-------
 public | weather | table | xutai
(1 row)

```



```
postgres=# \d weather
                      Table "public.weather"
 Column  |         Type          | Collation | Nullable | Default
---------+-----------------------+-----------+----------+---------
 city    | character varying(80) |           |          |
 temp_lo | integer               |           |          |
 temp_hi | integer               |           |          |
 prcp    | real                  |           |          |
 date    | date                  |           |          |
 ```


 ```
 postgres=# \d+ weather
                                          Table "public.weather"
 Column  |         Type          | Collation | Nullable | Default | Storage  | Stats target | Description
---------+-----------------------+-----------+----------+---------+----------+--------------+-------------
 city    | character varying(80) |           |          |         | extended |              |
 temp_lo | integer               |           |          |         | plain    |              |
 temp_hi | integer               |           |          |         | plain    |              |
 prcp    | real                  |           |          |         | plain    |              |
 date    | date                  |           |          |         | plain    |              |
Access method: heap
```

