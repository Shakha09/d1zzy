CREATE TABLE Employees (
    EmpID INT PRIMARY KEY,
    Name VARCHAR(50),
    Salary DECIMAL(10,2)
);

INSERT INTO Employees (EmpID, Name, Salary)
VALUES (1, 'Alice', 55000.00);

INSERT INTO Employees (EmpID, Name, Salary)
VALUES 
    (2, 'Bob', 60000.00),
    (3, 'Charlie', 70000.00);

UPDATE Employees
SET Salary = 7000.00
WHERE EmpID = 1;

DELETE FROM Employees
WHERE EmpID = 2;

ALTER TABLE Employees
MODIFY COLUMN Name VARCHAR(100);

ALTER TABLE Employees
ADD COLUMN Department VARCHAR(50);

ALTER TABLE Employees
MODIFY COLUMN Salary FLOAT;

CREATE TABLE Departments (
    DepartmentID INT PRIMARY KEY,
    DepartmentName VARCHAR(50)
);

TRUNCATE TABLE Employees;
