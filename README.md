# CRUD-Reactjs-Nodejs-Mysql
simple CRUD with reactjs nodejs mysql

# How to Run
    1. Clone this repository
    2. Export database
        run database: docker run --name ppm-mysql -e MYSQL_ROOT_PASSWORD=mysql -d mysql:latest
                      docker exec -it ppm-mysql bash
                      mysql --host 127.0.0.1 --port 33336 --user root -pmysql
    3. Open dir server-react
    4. Run server, type PORT=5500 node bin/www
    5. Back to root dir, then type npm-start
    6. Done. 

# Config database
goto server-react/bin/db.js then edit with yours
<pre>

    var connection = mysql.createConnection({
        host: 'localhost',
        user: 'root',
        password: '',
        database: 'db_mhs'
    });
</pre>