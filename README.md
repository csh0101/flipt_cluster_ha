# this is must

```sql

-- master --

exec SHOW MASTER STATUS

-- slave --
CHANGE MASTER TO
MASTER_HOST='mysql-master',
MASTER_USER='replica',
MASTER_PASSWORD='yourpassword',
MASTER_LOG_FILE='mysql-bin.xxxxxx',
MASTER_LOG_POS=xxx;
```
