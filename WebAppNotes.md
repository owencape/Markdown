# Web Application and Linux OS Notes





### Tips and Tricks
 - Logging into RPi -> ssh cs##@192.168.1.2##
  - if you cannot connect, check WiFi
  - if you lose connection, reconnect by firing another ssh command


### Commands 
 - Remove a folder or directory -> rmdir directoryName
 - Make a directory -> mkdir directoryName
 - Create an empty file -> touch filename
 - Open a text editor -> vim filename
 - mkdir -p path -> create multiple subfolders
 - concatenate a file to the terminal -> cat path/filename
 - to see all the items in a directory -> ls -a path
 - going -> cd ~
 - Temporary Root Access or Admin Privelege -> sudo -> super user do


### VIM Shortcuts
 - Go check the wiki page


### SQL Commands
|Definitions|Commands|
|---|---|
|Login to DB server| sudo mysql -u root -p|
|Close or exit server| ctrl c / ctrl d / exit|
|Password for root user| Password1|
|Create a db| CREATE DATABASE nameOfYourDB;|
| CRUD| Create, Read, Update, Delete|
| Create Data in DB| INSERT INTO TableName VALUES(data);|
| Obtain info from DB| SELECT fieldname FROM tableName|
| Update data in DB| UPDATE Tablename SET fieldata WHERE CLAUSE;|
| Remove data in DB| DELETE FROM TableName WHERE CLAUSE;|
|Update fields in a DB|ALTER TABLE Contacts ADD Email varchar(255);|



-----------------------------------------------------------------------
Create Table

  CREATE TABLE Contacts(
    Id int,
    LastName varchar(100),
    FirstName varchar(100)
  );

  CREATE TABLE States(
   Id int NOT NULL AUTO_INCREMENT,
   State varchar(2),
   PRIMARY KEY (Id),
   UNIQUE KEY (State)
  );


Insert into Table

  INSERT INTO Contacts VALUES(1, 'Doe', 'Jane');
  INSERT INTO Contacts VALUES(2, 'Payne', 'Max');

  INSERT INTO States (State) VALUES ('IN');
  INSERT INTO States (State) VALUES ('OH');


Update info

  UPDATE Contacts SET FirstName = 'Sweet', LastName='Caroline' WHERE Id = 1;

  UPDATE Contacts SET Email = 'sweetcaroline@neildiamondfanclub.com', StateId = 1 WHERE Id = 1;


Delete row

  DELETE FROM Contacts WHERE Id = 2;

Alter tables to add columns

  ALTER TABLE Contacts ADD Email varchar(255);

  ALTER TABLE Contacts ADD StateId int;





