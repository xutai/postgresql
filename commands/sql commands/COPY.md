D:\db\postgresql\data

/ represents  D:\


```sql
COPY (SELECT * FROM weather) TO '/postgresql-flat-text.txt';
COPY (SELECT * FROM weather) TO '/db/postgresql/data/postgresql-flat-text.txt';
```
```sql
COPY weather FROM '/db/postgresql/data/postgresql-flat-text.txt';
```


sample
```sql
COPY weather FROM '/home/user/weather.txt';
```

```sql
COPY weather FROM 'C:\Users\Administrator\postgresql-flat-text.txt'
COPY weather FROM 'postgresql-flat-text.txt'
COPY weather FROM './postgresql-flat-text.txt'
```

not working
```sql
COPY weather FROM '/postgresql-flat-text.txt'
```



flat-txt sample
```
San Francisco	57	43	0	1994-11-29
San Francisco	57	43	0	1994-11-29
```
