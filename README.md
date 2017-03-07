# We Todo Api

## Install Yo and We.js
```
npm install we yo generator-wejs -g
```

## On this project

1. Clone and install npm packages
    ```
    git clone https://github.com/ravuthz/we-todo-api.git todo-app
    cd todo-app
    npm install
    ```

2. Create database and then run it
    ```
    mysql -u ravuthz -e 'create database todo';
    we go
    ```

## Or create the new one

1. Generate todo app
    ```
    yo wejs
    ```

    Example Configure
    ```
    ? Your project name: todo
    ? Choice one database for your project: mysql
    ? Database name: todo
    ? Database user name: ravuthz
    ? Database password :
    ? Create the first user: yes
    ? User name: admin
    ? User email: admin@example.com
    ? User password: 123123
    ? User display name: Administrator
    ```

2. Create and configure database
    ```
    mysql -u ravuthz -e 'create database todo';
    ```

3. Configure configuration file
    ```
    config/local.js
    ```

4. Load the default locales
    ```
    we loadLocales
    ```

5. Generate the Task CRUD (model, controller, resource, test)
    ```
    yo wejs:resource task name:string done:boolean
    ```

NOTE:
* Start server
    ```
    we go
    ```

* Unit testing
    ```
    we test
    ```
