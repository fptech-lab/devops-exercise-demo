# What's inside
A simple php script (html/index.php) in order to:
- connect to a MySQL DB using environment variables:<br/>
    - MYSQL_HOST: hostname of database server
    - MYSQL_DATABASE: database name
    - MYSQL_USER: user that can connect to db
    - MYSQL_PASSWORD: password for MYSQL_USER
- moreover it creates a table named "hits"
- insert current client ip with timestamp inside this table
- show session details
<br/><br/>
# Exercise
Please complete the following steps:
1. create a docker compose/stack with two services:
    - db: mysql/mariadb
    - web: webserver of your choice to serve the php script
2. create public git repository to push your scripts
3. create an ansible playbook that runs tasks:
    - ensure target machine has prerequisites
    - get scripts from git repository
    - push file to target machine
    - run services on target machine
