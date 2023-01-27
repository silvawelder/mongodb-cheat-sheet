# mongodb-cheat-sheet

- [Login on MongoDB](#Login-on-MongoDB)
- [Manipulating Database](#Manipulating-Database)
  * [How to create a new database](#How-to-create-a-new-database)
  * [How to list all databases](#How-to-list-all-databases)
  * [How to use a database](#How-to-use-a-database)
- [Manipulating Collections](#Manipulating-collections)
  * [How to list all collections](#How-to-list-all-collections)
  * [How to list all collections from a schema](#How-to-list-all-collections-from-a-schema)
  * [How to delete a collection from a schema](#How-to-delete-a-collection-from-a-schema)
  * [How to delete all collections from a schema](#How-to-delete-all-collections-from-a-schema)

- [Manipulating Users](#Manipulating-collections)
  * [How to create a new user](#How-to-create-a-new-user)
  * [How to create a password to an user](#How-to-create-a-password-to-an-user)
  * [Grant privileges to an user](#Grant-privileges-to-an-user)
  * [List all users](#List-all-users)

- [Manipulating connections](#Manipulating-connections)
  * [List number of active connections and max connections](#List-number-of-active-connections-and-max-connections)
  * [How to create a password to an user](#How-to-create-a-password-to-an-user)
  * [Kill active connections](#Kill-active-connections)

    ## Login on MongoDB

    command:  
    ```
    mongo -u root -p --host <host-mongodb> --authenticationDatabase admin
    ```

    sample:  
    ```
    mongo -u root -p --host 10.0.0.16 --authenticationDatabase admin
    ```

    ## Manipulating Database

    ### How to create a new database
    command:
    ```
    use <db-name>;
    db.test.insert({field: "value"})
    ```

    sample:
    ```
    use my_db;
    db.test.insert({field: "value"})
    ```
    ### How to list all databases
    command:
    ```
    > show dbs;
    ```

    sample:
    ```
    > show dbs;
    admin                               0.000GB
    config                              0.000GB
    ```  
    ### How to use a database
    command:
    ```
    use <database_name>;
    ```

    sample:
    ```
    use admin;
    switched to db admin
    ```  
