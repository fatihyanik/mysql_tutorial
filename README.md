```jsx
Database:
Database is a structured collection of data that is organized so that it can be easily accessed managed and updated.
It is typically stored and managed using a specialized software called database management system or (DBMS).

```

```jsx
Veritabanı:
Veritabanı, kolayca erişilebilecek, yönetilebilecek ve güncellenebilecek şekilde organize edilmiş yapılandırılmış bir veri koleksiyonudur.
Genellikle veritabanı yönetim sistemi veya (DBMS) adı verilen özel bir yazılım kullanılarak saklanır ve yönetilir.
```

```jsx
DBMS:
DBMS stands for Database Management System. It is software that allows users to interact wit a database.
DBMSs are designed to manage large volumes of data efficiently and provide mechanisms for storing, retireving, updating, and managing that data.
```

```jsx
DBMS, Veritabanı Yönetim Sistemi anlamına gelir. Kullanıcıların bir veritabanı ile etkileşime girmesini sağlayan yazılımdır.
DBMSler büyük hacimli verileri verimli bir şekilde yönetmek için tasarlanmıştır ve bu verileri depolamak, geri almak, güncellemek ve yönetmek için mekanizmalar sağlar.
```

```jsx
SQL (STRUCTURED QUERY LANGUAGE):
It is a standardized language for managing relational databases.
You can use it to interact with various database system to insert, update, delete, and retrieve data.
```

```jsx
SQL (YAPILANDIRILMIŞ SORGU DILI):
İlişkisel veritabanlarını yönetmek için standartlaştırılmış bir dildir.
Veri eklemek, güncellemek, silmek ve almak için çeşitli veritabanı sistemleriyle etkileşim kurmak için kullanabilirsiniz.
```

```jsx
MYSQL:
An open source RDBMS (relational database management system) that uses SQL.
Think of it is as a database with SQL as its access language.
Other examples include Microsoft SQL server and Oracle Databases.
```

```jsx
MYSQL:
SQL kullanan açık kaynaklı bir RDBMS (ilişkisel veritabanı yönetim sistemi).
Erişim dili SQL olan bir veritabanı olarak düşünün.
Diğer örnekler arasında Microsoft SQL server ve Oracle Veritabanları bulunmaktadır.
```

```jsx
Analogy:
Imagine SQL as a common language you can  use to communicate with different librarians (relational database management systems).
MYSQL would be a specific library with its own collection (database) that you can access and manage using SQL commands.
```

```jsx
Analoji:
SQL'i farklı kütüphanelerle (ilişkisel veritabanı yönetim sistemleri) iletişim kurmak için kullanabileceğiniz ortak bir dil olarak düşünün.
MYSQL, SQL komutlarını kullanarak erişebileceğiniz ve yönetebileceğiniz kendi koleksiyonuna (veritabanı) sahip özel bir kütüphane olacaktır.
```

```jsx
Showing Databases
SHOW DATABASES;

Create Database
CREATE DATABASE NAME;

DROP / DELETE Database
DROP DATABASE NAME;

Getting Into Database / Using Database
USE DATABASE_NAME;

Which database we are currently using
SELECT DATABASE();

```

```jsx
TABLE:
Table is a collection of data organized in a rows and columns.
Tables are used to store and organize the data in a structured format, making it easier to retrieve and manipulate the data
```

```jsx
TABLO:
Tablo, satırlar ve sütunlar halinde düzenlenmiş bir veri koleksiyonudur.
Tablolar, verileri yapılandırılmış bir biçimde depolamak ve düzenlemek için kullanılır, bu da verilerin alınmasını ve işlenmesini kolaylaştırır
```

```jsx
DATA TYPES:
Datatype tells the database what kind of information can be store in a particular column.
For example, a column with data type of "integer" can only store the whole numbers, while a column with the datatype of "text" can store letters, numbers, and other characters.
```

```jsx
VERİ TÜRLERİ:
Veri türü, veritabanına belirli bir sütunda ne tür bilgilerin saklanabileceğini söyler.
Örneğin, veri türü "integer" olan bir sütun yalnızca tam sayıları depolayabilirken, veri türü "text" olan bir sütun harfleri, sayıları ve diğer karakterleri depolayabilir.
```

```jsx
CREATE TABLE GAMES(
    name VARCHAR(50)
    ratings INT
)

Create a new table name "GAMES". The table has two columns: "name" and "age".

name: can store variable-length character strings with a maximum length of 50 characters.
ratings: can store whole numbers.
```

```jsx
Display a list of all tables in a database
SHOW TABLES;

Display the columns (fields) of a table (TABLE NAME)
SHOW COLUMN NAME;


Display / Describe the structure of a table
DESC NAME;

Add Default Values
CREATE TABLE GAMES (
    name VARCHAR(50) DEFAULT 'Anonymous',
    release INT DEFAULT 2024,
    ratings INT
)

Drop / Delete Table
DROP TABLE NAME;
```

```jsx
CHAR(size):
CHAR is used for fixed-length character strings. When you define a CHAR column, you must specify a fixed length for the string, e.g., CHAR(10). If you store a shorter string in a CHAR(10) column, it will be padded with spaces to fill the fixed length.
```

```jsx
CHAR(size):
CHAR, sabit uzunluktaki karakter dizeleri için kullanılır. Bir CHAR sütunu tanımladığınızda, dize için sabit bir uzunluk belirtmelisiniz, örneğin CHAR(10). CHAR(10) sütununda daha kısa bir dize saklarsanız, sabit uzunluğu doldurmak için boşluklarla doldurulacaktır.
```

```jsx
VARCHAR(size):
VARCHAR, is used for variable-length character strings. When you define a VARCHAR column, you specify a maximum length for the string, e.g., VARCHAR(255).
The actual storage size of the string is the length of the data plus one byte to store the length of the data. This means that VARCHAR can store variable-length strings efficiently without padding.
```

```jsx
VARCHAR(boyut):
VARCHAR, değişken uzunluktaki karakter dizeleri için kullanılır. Bir VARCHAR sütunu tanımladığınızda, dize için maksimum bir uzunluk belirtirsiniz, örneğin, VARCHAR(255).
Dizenin gerçek depolama boyutu, verinin uzunluğu artı verinin uzunluğunu saklamak için bir bayttır. Bu, VARCHAR ın değişken uzunluktaki dizeleri dolgu olmadan verimli bir şekilde depolayabileceği anlamına gelir.
```

```jsx
INT:
INT is used to store whole numbers (integers) without decimal points.
```

```jsx
INT:
INT, ondalık noktasız tam sayıları (tamsayılar) saklamak için kullanılır.
```

```jsx
DECIMAL:
DECIMAL datatype is used to store exact numeric values. It is commonly used for monetary or other values where precision is required.
The DECIMAL datatype requires two parameters: DECIMAL(p,s), where p specifies the total number of digits that can be stored (precision), and a specifies the number of digits after the decimal point (scale).
```

```jsx
DECIMAL:
DECIMAL veri tipi tam sayısal değerleri saklamak için kullanılır. Genellikle parasal veya hassasiyetin gerekli olduğu diğer değerler için kullanılır.
DECIMAL veri türü iki parametre gerektirir: DECIMAL(p,s), burada p saklanabilecek toplam basamak sayısını (hassasiyet) ve a ondalık noktadan sonraki basamak sayısını (ölçek) belirtir.
```

```jsx
DATE:
Stores a date value in the format 'YYYY-MM-DD'
For example, '2024-03-02' represent March 2, 2024.
```

```jsx
TIME:
Stores a time value in the format 'HH-MM-SS'
For example, '14:30:00' represent March 2.30.00.
```

```jsx
DATETIME:
DATATIME datatypes is used to Store both date and a time information in the format.
For example, 'YYYY-MM-DD HH:MM:SS'
```

```jsx
Insert Data Label(s)
INSERT INTO games(name, ratings);
```

```jsx
Provide Values For Label(s)
VALUES ('GTA 6', 6)
```

```jsx
Multible Values Insert
VALUES ('GTA 6', 6)
       ('Batman Knight', 8)
        ('AKR 2', 1)
```

```jsx
Select specific property from a table
SELECT PROPERTY FROM TABLE;

SELECT ratings FROM games;
```

```jsx
Select multiple properties from a table
SELECT PROPERTY1, PROPERTY2 FROM TABLE;

SELECT name, ratings FROM games;
```

```jsx
PRIMARY KEYS:
A primary key is a unique identifier for each record in a table.
It ensures that each row in a table is uniquely identifiable and helps maintain the integrity of the data.
A primary key column cannot have NULL values, and each value in the column must be unique.
```

```jsx
BİRİNCİL ANAHTARLAR:
Birincil anahtar, bir tablodaki her kayıt için benzersiz bir tanımlayıcıdır.
Bir tablodaki her satırın benzersiz bir şekilde tanımlanabilmesini sağlar ve verilerin bütünlüğünün korunmasına yardımcı olur.
Bir birincil anahtar sütunu NULL değerlere sahip olamaz ve sütundaki her değer benzersiz olmalıdır.
```

```jsx
WHERE:
WHERE keyword is used to filter records that meet a specified condition. It is typically used in SELECT, UPDATE, and DELETE statements to narrow down the results or specify which rows to update or delete.
```

```jsx
WHERE:
WHERE anahtar sözcüğü, belirli bir koşulu karşılayan kayıtları filtrelemek için kullanılır. Genellikle SELECT, UPDATE ve DELETE deyimlerinde sonuçları daraltmak veya hangi satırların güncelleneceğini veya silineceğini belirtmek için kullanılır.
```

```jsx
Select all games where ratings is 5
SELECT * FROM games WHERE ratings=5;
```

```jsx
Give me the names of those games who's ratings is 5
SELECT name FROM games WHERE ratings=5;
```

```jsx
Provide Alias For Specific Item
SELECT id AS game_id FROM DATING_APP;
```

```jsx
Update Data
UPDATE table_name
SET column1=value1, column2=value2...
WHERE condition;
```

```jsx
table_name : The name of the table you want to update.
columns : The columns you want to update.
values : The new values you want to set for the columns.
condition: The condition that specifies which rows to update. If omitted, al rows will be updated. 
```

```jsx
UPDATE users
SET age = 30
WHERE id = 1;
```

```jsx
Delete Column From the Table
DELETE FROM table_name
WHERE condition;
```

```jsx
DELETE FROM users
WHERE id=1;
```

```jsx
Delete Everthing / Clear The Table
DELETE FROM users;
```

```jsx
SUBSTRING() Function
SUBSTRING() function is used to extract a substring from a string.
It allows you to specify the starting position and the length of the substring to extract.

SUBSTRING(string, start_position, length)
```

```jsx
SELECT SUBSTRING('Murat', 1, 3)
```

```jsx
CREATE TABLE employees (
    id INT PRIMARY KEY,
    first_name VARCHAR(50),
    last_name VARCHAR(50),
    department VARCHAR(50),
    salary DECIMAL(10, 2)
);

INSERT INTO employees (id, first_name, last_name, department, salary)
VALUES
    (1, 'John', 'Doe', 'IT', 50000.00),
    (2, 'Jane', 'Smith', 'HR', 60000.00),
    (3, 'Alice', 'Johnson', 'Finance', 70000.00);

-- Create a view
CREATE VIEW employee_names AS
SELECT id, CONCAT(first_name, ' ', last_name) AS full_name
FROM employees;

-- Query the view
SELECT * FROM employee_names;

-- Update the view (recreate it)
-- Create a view if didn't exists already, or replace it with this new one.

CREATE OR REPLACE VIEW employee_names AS
SELECT id, CONCAT(first_name, ' ', last_name) AS full_name
FROM employees
WHERE department = 'IT';

SELECT * FROM employee_names;

-- Delete the view
DROP VIEW employee_names;
```