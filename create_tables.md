# CREATE TABLE Employee

```sql

CREATE TABLE Employee( 
    EmpNo INT(3) PRIMARY KEY, 
    EName VARCHAR(35) NOT NULL, 
    jCode INT(3) REFERENCES Job(jCode), 
    MgrNo INT(3) REFERENCES Employee(EmpNo), 
    HireDate DATE, 
    Salary INT(10), 
    Commission FLOAT(11,2), 
    DeptNo INT(3) REFERENCES Department(DeptNo)
);


### Insert into Employee

INSERT INTO Employee VALUES (1, 'venkat', 672, NULL, '2006-02-01', 1200000, 10000, 40);
INSERT INTO Employee VALUES (2, 'Nirmala', 671, 1, '2007-04-02', 800000, 50000, 20);
INSERT INTO Employee VALUES (3, 'Pradeep', 669, 1, '2005-10-10', 1000000, NULL, 40);
INSERT INTO Employee VALUES (4, 'Srinivas', 669, 1, '2005-05-08', 1000000, NULL, 30);
INSERT INTO Employee VALUES (5, 'Krishna', 668, 2, '2005-10-09', 500000, 20000, 22);
INSERT INTO Employee VALUES (6, 'Deepa', 668, 3, '2007-09-09', 600000, NULL, 23);
INSERT INTO Employee VALUES (7, 'Keerthi', 668, 4, '2006-06-05', 600000, NULL, 24);
```

---

# CREATE TABLE Department

```sql
CREATE TABLE Department( 
    DeptNo INT(3) PRIMARY KEY, 
    DName VARCHAR(35), 
    LCode INT(3) REFERENCES Location(lCode)
);
```

### Insert into Department

```sql
INSERT INTO Department VALUES (10, 'Accounting', 122);
INSERT INTO Department VALUES (20, 'Research', 124);
INSERT INTO Department VALUES (30, 'Sales', 123);
INSERT INTO Department VALUES (40, 'Operations', 167);
INSERT INTO Department VALUES (22, 'Finance', 122);
INSERT INTO Department VALUES (23, 'Sales', 122);
INSERT INTO Department VALUES (24, 'HR', 122);
```

---

# CREATE TABLE Job

```sql
CREATE TABLE Job( 
    JCode INT(3) PRIMARY KEY, 
    JName VARCHAR(35) NOT NULL
);
```

### Insert into Job

```sql
INSERT INTO Job VALUES (666, 'Clerk');
INSERT INTO Job VALUES (667, 'Trainee');
INSERT INTO Job VALUES (668, 'Analyst');
INSERT INTO Job VALUES (669, 'SalesPerson');
INSERT INTO Job VALUES (670, 'Manager');
INSERT INTO Job VALUES (671, 'President');
```

---

# CREATE TABLE Location

```sql
CREATE TABLE Location( 
    lCode INT(3) PRIMARY KEY, 
    lName VARCHAR(35) NOT NULL
);
```

### Insert into Location

```sql
INSERT INTO Location VALUES (122, 'Chicago');
INSERT INTO Location VALUES (123, 'Atlanta');
INSERT INTO Location VALUES (124, 'NewYark');
INSERT INTO Location VALUES (167, 'Paris');
```
