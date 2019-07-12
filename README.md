# Generators - test task

[![N|Solid](https://cdn1.savepice.ru/uploads/2019/7/12/2ab3c1832b7957689c4355606e4b09f9-full.png)](https://cdn1.savepice.ru/uploads/2019/7/12/2ab3c1832b7957689c4355606e4b09f9-full.png)

### Instructions

1. Create table in your data base and execute INSERT SQL query:

```sql
CREATE TABLE IF NOT EXISTS `test` (
  `sum` varchar(500) DEFAULT NULL,
  `count_fib` smallint(6) DEFAULT NULL,
  `count_prime` smallint(6) DEFAULT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8;

INSERT INTO test SET sum = '0', count_fib = 0, count_prime = 0;
```
2. redis-cli must be installed. See [https://redis.io/download](https://redis.io/download)
3. Set DB connection params in Constants.php
4. Run in concole
```sh
$ php runMulti.php
```
or
```sh
$ ./runMulti.sh
```