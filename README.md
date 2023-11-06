## Ex. No: 4 Creating Procedures using PL/SQL
## Date:
### AIM: To create a procedure using PL/SQL.

### Steps:
1. Create employee table with following attributes (empid NUMBER, empname VARCHAR(10), dept VARCHAR(10),salary NUMBER);
2. Create a procedure named as insert_employee data.
3. Inside the procdure block, write the query for inserting the values into the employee table.
4. End the procedure.
5. Call the insert_employee data procedure to insert the values into the employee table.
6. Display the employee table

### Program:

```
 create table employee(empID int, empname char(10), dept char(20), salary int);
 Table created.

 create or replace procedure insert_employee_data as
 begin
 insert into employee values(1,'John','HR',50000);
 insert into employee values(2,'joe','IT',60000);
 insert into employee values(3,'Bob','Finance',55000);
 commit;
 end;
 /
 Procedure created.

 begin
 insert_employee_data;
 end;
  /
 PL/SQL procedure successfully completed.

 select * from employee;
```

### Output:

![image](https://github.com/Sujithra-dhayalan/Ex-No-4-Creating-Procedures-using-PL-SQL/assets/115523950/764e2cf0-83b4-4da6-b9c1-86ca37e6a87f)


### Result:
Hence a procedure using  SQL is created successfully. 

