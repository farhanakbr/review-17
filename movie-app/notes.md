
## STEP BY STEP LIVECODE
(**OOP - MVC(EXPRESS) - PG - CALLBACK**)

1. cd folder => npm init -y
2. npm i pg express ejs 
3. npm i -D nodemon
4. .gitignore => node_modules => (-10)
5. mkdir config controllers models views
6. touch connection.js setup.js seeding.js controller.js model.js app.js home.ejs

<br> **DATABASE** <br>
<br>7. edit => connection.js (https://node-postgres.com/features/connecting)
<br>8. setup.js / seeding.js => create table => 1 : M (FK)
<br>=> 1 : M (nested callback => pool.query)
<br>=> (https://www.postgresqltutorial.com/postgresql-create-table/)
<br>=> setup, table pake `""`, id serial, `FK(columnfk) - REFERENCES "Table"(pk)`
<br>=> (https://www.postgresqltutorial.com/postgresql-insert-multiple-rows/)
<br>=> seeding gaboleh masukin **id**, varchar pake `''`
<br>9. pastikan di DB

<br>**SERVER**<br>
<br>10. R0: buat class Model sesuaikan dengan views/table ejs soal
<br>11. set app.js => tanpa routes 
<br>   => (http://expressjs.com/en/starter/hello-world.html)
<br>   => set `('view engine', 'ejs')`
<br>   => use / middlewares `(express.urlencoded({extended: false}))`


<br>12. buat routes di app (.get & .post)
<br>13. buat class Controller, module.exports; require di app.js
<br>14. pindahin handler function `(req,res)` di static Controller
<br>15. buat `class Model` module.exports; require di controller.js
<br>16. handle routes dari home `.get('/')`




