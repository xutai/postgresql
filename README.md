postgresqltutorial.com


- add binary file folder to PATH E:\apps\postgresql\installer\pgsql\bin

- create data directory D:\db\postgresql\data

- then
```bash
initdb -D D:\\db\\postgresql\\data
```

- check data directory

- start the db server
```bash
postgres -D D:\\db\\postgresql\\data
```

- create db
```bash
createdb xutai
```

- access db
```bash
psql xutai
```

- try some commands
```bash
select version();
```