## Deskripsi Projek

Adalah Tugas Challenge Chapeter 4 memuat terkait Express.Js, database Prosgresql, ORM dan Asyncronous Process dalam perojek kali ini membuat sebuah website lanjutan dari projek sebelumnya projek ini yaitu BINAR CAR MANAGEMENT dalam projek ini dapat me manajemen data mobil CRUD : CREATE, READ, UPDATE, DELETE. dan web tersebut telah menggunakan HTTP Server dan beberapa kriteria lainnya.

## ERD Database

![Alt text](/ERD_Binar.png)

## Cara penggunaan

1. npm init
   utk start project node js kita

2. npm install express morgan nodemon pg pg-hstore sequelize sequelize-cli
   morgan utk logger
   nodemon utk otomatis restart server, kalau ada perubahan di project
   sequelize itu ORM, library yang ngebuat kita lbh mudah mengelola database

3. configurasi package.json kita, tambahin script dev : nodemon index.js/server.js
   kalau error, akalin dengan script baru atau langsund di terminal nodemon index.js

4. npx sequelize init
   utk start sequelize config di project kita

5. npx sequelize model:generate --name product --attributes name:string,price:integer,stock:integer
   generate model atau table untuk database kita

6. npx sequelize db:create
   perintah untuk bikin/create db baru sesuai nilai dari database yg ada di config.json

7. npx sequelize db:migrate
   perintah untuk migration table/model yang udh kita generate sebelumnya
