# create database studentdb
# create table tblstudent
## columns are
1.studentId  datatyepe integer , make it as primary key and it shiuld be auto incremented,
2.studentName datatyepe varchar, range 64
3.dob datatyp date,
4. address datatyp varchar range 64

## Add atlead three entries (3 rows) into the table


-- Create the studentdb database

CREATE DATABASE studentdb;

-- Switch to the studentdb database

USE studentdb;

-- Create the tblstudent table

CREATE TABLE tblstudent (
    studentId INT PRIMARY KEY AUTO_INCREMENT,
    studentName VARCHAR(64),
    dob DATE,
    address VARCHAR(64)
);

-- Add three entries into the tblstudent table

INSERT INTO tblstudent (studentName, dob, address) VALUES
('John Doe', '1990-05-15', '123 Main St'),
('Jane Smith', '1992-08-25', '456 Oak Ave'),
('Bob Johnson', '1995-02-10', '789 Elm Blvd');
