To load a schema into a database

`mysql -p -D DBNAME < SCHEMAFILE`

To grant access to a specific database for a user/password

`grant all on DB.* to 'USER'@'DOMAIN' identified by 'PASSWORD';`

To load a csv file of data into a table

`load data local infile FILE into table TABLE [fields termintated by 'DELIMETER'];`
