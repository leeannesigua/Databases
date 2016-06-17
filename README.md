# Databases

LAB 1: 
1. Using SQL create a table called empbb02 with columns EMPNO, ENAME, POS, BOSS, HIREDATE, SAL, DEPTNO, and INCENTIVES. Input data into that table given by instructor.
2. Create a table called infobb02 with columns EMPNO, FNAME, NICK, UNI, AVERAGE, ERA. Input data in that table given by instructor.
3. Create a table called debtbb02 with columns DEBTNO, DNAME, RESTAURANT, LOCATION, MOTTO. Input data in that table given by instructor.
4. Create a table called salsbb02 with columns GRADE, ROLE, LOSAL, HISAL. Input data in that table given by instructor.

LAB 2:
1. Display user_constraints for empno and deptno
2. Test Primary Constraint for deptno by entering a row with null for deptno in deptbb02
SQL> INSERT INTO deptbb02 VALUES (null, 'outfield', 'The Shack', 'Miramar', 'Get your grub on');
INSERT INTO deptbb02 VALUES (null, 'outfield', 'The Shack', 'Miramar', 'Get your grub on')
3. Display user_constraints for salsbb02
4. Display deptbb02, make sure motto column does not wrap
5. Test Check Constraint. Try to 'hire' Dan Quiesenberry.
6. In the terminology of foreign keys, you should not be alloed to drop a parent table, if it still has children. Verify this using your tables.

LAB 3:
1a. Display last name, first name, and department name for all employees not in department 40 or 50.
1b. Make a relational algebra expression based on 1a.
2. Output lines for each department.
3. Create a copy of empbb02 called tempbb02.
4. Using tempbb02, add to each employee salary his department number.
5. Using tempbb02, add to each employee salary his uniform number.
6. The boss is asking for last name, salary, and position of all employees making more than the highest paid pitcher.
7a. Display each employee by name, with years and months of service.
7b. Add Jackie Robinson to the team, using empbb02 and infobb02.
8. Add "spouse" column to infobb02. Make value NA for each employee except Jackie Robinson. Then add Jackie Robinson's wife to the table.
9. Change new column name to "wife" and remove new column.

LAB 4: 
Part 1:
1. Create a table named blobclob with columns CLOBID, CLOB_COL, BLOB_COL.
Part 2:
1. SQL code to make the cdv files
2. Display the cdv files themselves
3. Display the 4 control files
4. Display the code to run sqlldr 4 times to fill tables
5. A spool file showing your entering the right schema, and then doing desc, and select * for all 4 tables.

LAB 5:
1. output all possible pairs where the first player is a coach and the second an infielder.
2a. Create a stored function whose input is a player last name and whose output is the uniform number of that player.
2b. Write a script (unix file with sql extension) that calls this function for mungo.
3a. Write a stored procedure whose input is a player last name and whose outputs are the appropriate restaurant and location.
3b. Test it.
4. Arrange to invoke the procedure you stored in 3. above from a java jdbc program and test it.
