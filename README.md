## Methods and Objects

### ClickHouse
`` `php
public __constuct ([String $ protocol = "http" [, String $ host = "127.0.0.1" [, int $ port = 8123 [, $ user = null [, $ pass = null]]]]]): ClickHouse
``
Sets parameters for connecting to the database.


- $ protocol - Protocol for connecting to the base (http or https)
- $ host - Database host
- $ port - Database port
- $ user - Database username
- $ pass - Database user password

`` `php
public query (String $ query): ClickHouseData
``
Executes an SQL query and returns a result set as a ClickHouseData object.


### ClickHouseData
`` `php
public execute ([$ args]): ClickHouseData
``
Runs a prepared statement. If the request contains parameter markers (pseudo-variables), you must pass an array of values ​​as input only.

- $ args - An array of values ​​containing as many elements as the parameters are declared in the SQL query.
