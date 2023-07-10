# SmartParking
IBM Internship Exercise: Cloud Native Application Developer

**The app is built with Node.js, Vue, MySQL.**
API from  https://platerecognizer.com is used in order to recognize plate numbers and compare the images.
The API requires a key, which can be gained on their site.
It should be entered in the platerecognizer.js in place of  ***your token***.

In order to install necessary packages run:
```
$ npm install axios express multer mysql2
```

MySQL server needs to be running. Please, look in the mysql.js to fill in the information. In order to create database run:
```
CREATE DATABASE SmartParking;
```
In order to create table used by mysql.js module run:
```
CREATE TABLE PlateData (
  id INT NOT NULL AUTO_INCREMENT,
  fee INT NOT NULL,
  duration INT NOT NULL,
  hours INT NOT NULL,
  vehicleType VARCHAR(255) NOT NULL,
  typestamp1 TIMESTAMP NOT NULL,
  typestamp2 TIMESTAMP NOT NULL,
  PRIMARY KEY (id)
);
```
App can be ran with:
```
$ node app.js
```


