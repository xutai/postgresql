try`initdb -D D:\db\postgresql\data`

```bash
$ initdb -D D:\db\postgresql\data
The files belonging to this database system will be owned by user "Administrator".
This user must also own the server process.

The database cluster will be initialized with locale "English_United States.936".
Encoding "GBK" implied by locale is not allowed as a server-side encoding.
The default database encoding will be set to "UTF8" instead.
The default text search configuration will be set to "english".

Data page checksums are disabled.

creating directory D:dbpostgresqldata ... ok
creating subdirectories ... ok
selecting dynamic shared memory implementation ... windows
selecting default max_connections ... 20
selecting default shared_buffers ... 400kB
selecting default time zone ... Asia/Hong_Kong
creating configuration files ... ok
running bootstrap script ... E:/apps/postgresql/installer/pgsql/bin/postgres.exe: could not access directory "C:/Users/Administrator/D:dbpostgresqldata": No such file or directory
Run initdb or pg_basebackup to initialize a PostgreSQL data directory.
child process exited with exit code 1
initdb: removing data directory "D:dbpostgresqldata"
```

try `initdb -D D:\\db\\postgresql\\data`

u will get
```bash
$ initdb -D D:\\db\\postgresql\\data
The files belonging to this database system will be owned by user "Administrator".
This user must also own the server process.

The database cluster will be initialized with locale "English_United States.936".
Encoding "GBK" implied by locale is not allowed as a server-side encoding.
The default database encoding will be set to "UTF8" instead.
The default text search configuration will be set to "english".

Data page checksums are disabled.

fixing permissions on existing directory D:/db/postgresql/data ... ok
creating subdirectories ... ok
selecting dynamic shared memory implementation ... windows
selecting default max_connections ... 100
selecting default shared_buffers ... 128MB
selecting default time zone ... Asia/Hong_Kong
creating configuration files ... ok
running bootstrap script ... ok
performing post-bootstrap initialization ... ok
syncing data to disk ... ok

initdb: warning: enabling "trust" authentication for local connections
You can change this by editing pg_hba.conf or using the option -A, or
--auth-local and --auth-host, the next time you run initdb.

Success. You can now start the database server using:

    E:/apps/postgresql/installer/pgsql/bin/pg_ctl -D ^"D^:^\db^\postgresql^\data^" -l logfile start
```