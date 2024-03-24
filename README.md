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