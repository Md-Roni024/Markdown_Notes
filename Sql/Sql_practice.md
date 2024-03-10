- Left Join
  - SQL <span style="color:red;">lEFT JOIN </span> joins two tabble based on common column. Select all rows from left column and only common rows from right.
  <img src="left_join.png">
  - Left Join Code
    ```Sql
    SELECT Customers.customer_id, Customers.first_name, Orders.amount
    FROM Customers
    LEFT JOIN Orders
    ON Customers.customer_id = Orders.customer
    ```
  - left Join example:
  <img src="left_join2.png">

- INNER JOIN
    - The INNER JOIN command returns rows that have matching values in both tables.
    - <img src="inner_join.png">
    - Code:
    ```sql
    SELECT Customers.customer_id, Customers.first_name, Orders.amount
    FROM Customers
    JOIN Orders
    ON Customers.customer_id = Orders.customer;
    ```
    - Inner Join Example:
    <img src="inner_join2.png">

- Cross Join
  - In SQL, a Cross Join is also called a Cartesian Join, it performs cross product of records of two or more joined tables.
  - <img src="cross.png">
- 1581. Customer Who Visited but Did Not Make Any Transactions
  - ```sql
    SELECT v.visit_id,v.customer_id,t.transaction_id,t.amount from Visits v left join Transactions t on v.visit_id = t.visit_id
    ```
  - <img src="1581_left_join.png">
  - ```sql
    SELECT customer_id, COUNT(v.visit_id) as count_no_trans from Visits v left join Transactions t on v.visit_id = t.visit_id where transaction_id IS NULL GROUP BY customer_id 
    ```

- 1280. Students and Examinations
  ``` sql
  SELECT * from Students cross join Subjects
  ```
  <img src="1280_cross.png">

  ```sql
  SELECT student_id,subject_name,COUNT(subject_name) AS CNT FROM Examinations GROUP BY student_id,subject_name
  ```
  <img src="1280_cross2.png">