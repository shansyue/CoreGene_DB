## Main Direction :

genomes -> BLASTp on Linux -> many BLASTp reports ( includes similarity, e-value, % overlapping ... to define "similar" )

->

get .txt from BLASTp -> store in MySQL -> new score ( based on BLAST report ) to summary in DB ( MCL paper ) 
-> get similar gene ( core gene candidate, use DEG to validate ) -> get core gene -> GUI webpage oriented to find core gene 

## Webpage Spec :

### input :

e-value, scores, % overlapping ...

DNA seq needed to be compared with 

### output :

core gene

## Front-end :

Lang : HTML + CSS + Javascript

Tool : jQuery, mootools, AngularJS, ReactJS, Gulp

## Back-end :

PHP (Lang) +  (Server) + MySQL (DB)

## DB :

MySQL Root password : 3yh%#Gmd$n

Username : katelo, Pw : 0513311

## Ref :

- [SQLite vs MySQL vs PostgreSQL：关系型数据库比较](http://www.infoq.com/cn/news/2014/04/sqlite-mysql-postgresql)

- [簡單的 MySQL 使用教學](https://jerrynest.io/mysql-tutorial/)

- [MySQL 超新手入門](http://www.codedata.com.tw/category/database/5)

- [How to import data from text file to mysql database](https://stackoverflow.com/questions/13579810/how-to-import-data-from-text-file-to-mysql-database)

- 


