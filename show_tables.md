Here’s how your SQL data and queries can be represented in Markdown format:

```sql
-- Table: Department
SELECT * FROM Department;

+--------+------------+-------+
| DeptNo | DName      | LCode |
+--------+------------+-------+
|     10 | Accounting |   122 |
|     20 | Research   |   124 |
|     22 | Finance    |   122 |
|     23 | Sales      |   122 |
|     24 | HR         |   122 |
|     30 | Sales      |   123 |
|     40 | Operations |   167 |
+--------+------------+-------+
7 rows in set (0.00 sec)
```

```sql
-- Table: Employee
SELECT * FROM Employee;

+-------+----------+-------+-------+------------+---------+------------+--------+
| EmpNo | EName    | jCode | MgrNo | HireDate   | Salary  | Commission | DeptNo |
+-------+----------+-------+-------+------------+---------+------------+--------+
|     1 | venkat   |   672 |  NULL | 2006-02-01 | 1200000 |   10000.00 |     40 |
|     2 | Nirmala  |   671 |     1 | 2007-04-02 |  800000 |   50000.00 |     20 |
|     3 | Pradeep  |   669 |     1 | 2005-10-10 | 1000000 |       NULL |     40 |
|     4 | Srinivas |   669 |     1 | 2005-05-08 | 1000000 |       NULL |     30 |
|     5 | Krishna  |   668 |     2 | 2005-10-09 |  500000 |   20000.00 |     22 |
|     6 | Deepa    |   668 |     3 | 2007-09-09 |  600000 |       NULL |     23 |
|     7 | Keerthi  |   668 |     4 | 2006-06-05 |  600000 |       NULL |     24 |
+-------+----------+-------+-------+------------+---------+------------+--------+
7 rows in set (0.00 sec)
```

```sql
-- Table: Job
SELECT * FROM Job;

+-------+-------------+
| JCode | JName       |
+-------+-------------+
|   666 | Clerk       |
|   667 | Trainee     |
|   668 | Analyst     |
|   669 | SalesPerson |
|   670 | Manager     |
|   671 | President   |
+-------+-------------+
6 rows in set (0.01 sec)
```

```sql
-- Table: Location
SELECT * FROM Location;

+-------+---------+
| lCode | lName   |
+-------+---------+
|   122 | Chicago |
|   123 | Atlanta |
|   124 | NewYark |
|   167 | Paris   |
+-------+---------+
4 rows in set (0.00 sec)
```

### Common Error

If you receive errors like:

```
ERROR 1064 (42000): You have an error in your SQL syntax...
```

It could be caused by incorrect copying and pasting of commands. Make sure each SQL command is written on its own and without additional prompts or shell outputs from previous commands.