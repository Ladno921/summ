# Введение в системы управления базами данных 

СУБД — комплекс программ, позволяющих создать базу данных (БД) и манипулировать данными (вставлять, обновлять, удалять и выбирать). Система обеспечивает безопасность, надёжность хранения и целостность данных, а также предоставляет средства для администрирования БД.

## СУБД MySQL

    https://www.mysql.com/

## SQL

SQL (аббр. от англ. Structured Query Language — «язык структурированных запросов») — декларативный язык программирования, применяемый для создания, модификации и управления данными в реляционной базе данных, управляемой соответствующей системой управления базами данных.

Просмотр листинга баз данных

    show databases;

Пример создания базы данных

    create database nature;

Подключить базу данных

    use database;

Просмотр листинга таблиц БД

    show tables;

Пример создания таблицы в БД

    create table items (id int primary key auto_increment, title varchar(255), image varchar(255));

Просмотр структуры таблицы БД

    describe items;

Выборка данных

    SELECT * FROM <table>;

Выборка данных с условием

    SELECT * FROM <table> WHERE <column>=<value>;

Запись данных в БД

    INSERT INTO <table> (<column>, <column>) VALUES ('<value>', '<value>');

Обновить запись в БД

    UPDATE <table> SET <column>=<value>;

Удалить запись из БД

    DELETE FROM <table> WHERE <column>=<value>;

Удаление таблицы 

    drop table items;

Изменение типа столбца в БД

    Alter table items modify column description varchar(32000);

Добавление столбца в БД

    alter table items add description varchar(255) after image;

