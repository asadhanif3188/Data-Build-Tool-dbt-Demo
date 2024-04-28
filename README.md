# Data-Build-Tool-dbt-Demo

## dbt-adapter for MySql 
Following is the sample profile (`~/.dbt/profiles.yml`) for mysql dbt-adapter
```
your_profile_name:
  target: dev
  outputs:
    dev:
      type: mysql
      server: localhost
      port: 3306
      schema: db_name
      username: your_mysql_username
      password: your_mysql_password
      ssl_disabled: True
```

## Test the connectivity of profile with dbt-adapter 
To test the connectivity of profile to mysql dbt-adapter, use following command. 

```
dbt debug 
```

## Running the models 
Following command is used to run all defined models.
```
dbt run
``` 

