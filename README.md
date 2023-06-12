# Exp 08 - IMPLEMENTATION OF THE KEYWORDS
[CROSS,CASE,JOIN,FULL OUTER JOIN]

## AIM:

To implement CASE,CROSS,JOIN,FULL OURT JOIN in SQL.

## ALGORITHM:

1) Create a sample table in SQL using CREATE TABLE syntax
2) Insert all the values and Titles respectively using INSERT INTO syntax
3) Now check whether all the rows are affected or not by fetching the table
4) After checking, now use SELECT for choosing the column name that we want and use FROM to choose the table
5) Then use CASE,CROSS,JOIN,FULL OURT JOIN syntax to implement its functionality.
6) After compiling and running the program, the results will be displayed.

## PROGRAM:

### TABLE:

```java
CREATE TABLE EMPLOYEE(
 	SNO int,
	FNAME varchar(50),
  	LNAME varchar(50),
	SALARY int
);
INSERT INTO EMPLOYEE VALUES (1,'John','MCFlury',8000);
INSERT INTO EMPLOYEE VALUES (2,'Vols','Vegan',4000);
INSERT INTO EMPLOYEE VALUES (3,'Amilia','Doofenshmirt',5000);
INSERT INTO EMPLOYEE VALUES (4,'Camilia','Jordan',3000);
INSERT INTO EMPLOYEE VALUES (5,'Max','Zeus',4500);
INSERT INTO EMPLOYEE VALUES (6,'Jacob','Norway',6700);
INSERT INTO EMPLOYEE VALUES (7,'Becky','Rodgerd',10000);
SELECT *FROM EMPLOYEE;

```

### CASE:

```java
SELECT SALARY ,
CASE
	WHEN SALARY <= 3000 THEN 'LOW'
    WHEN SALARY > 3000 AND SALARY <= 5000 THEN 'AVG'
    ELSE 'HIGH'
END AS PREDICT
FROM EMPLOYEE
```

### FULL OUTER JOIN:

```java

SELECT FRUITS.basket_id, BASKET.basket_id
FROM FRUITS
FULL OUTER JOIN BASKET ON FRUITS.basket_id=BASKET.basket_id
ORDER BY FRUITS.basket_id;

```
### CROSS JOIN:

```java

SELECT SalesOrg.sales_org , Channel.channel
FROM SalesOrg
CROSS JOIN Channel;

```

### JOIN:
```java

SELECT SalesOrg.sales_id , Channel.channel_id
FROM SalesOrg
JOIN Channel;

```

## OUTPUT:

### CASE:

<img width="292" alt="e8 1" src="https://github.com/divvisha/IMPLEMENTATION-OF-KEYWORD/assets/127508123/07073fa1-ae8e-4ae5-a0c5-dfc9ca7aeecb">

### FULL OUTER JOIN:

<img width="615" alt="e8 2" src="https://github.com/divvisha/IMPLEMENTATION-OF-KEYWORD/assets/127508123/9e3a74c8-cfe3-4b4f-bea9-6fc6e8242b65">

### CROSS JOIN:

<img width="462" alt="e8 3" src="https://github.com/divvisha/IMPLEMENTATION-OF-KEYWORD/assets/127508123/96fc887c-6b29-4744-9d54-35f4e37899ab">

### JOIN:

<img width="210" alt="e8 4" src="https://github.com/divvisha/IMPLEMENTATION-OF-KEYWORD/assets/127508123/b644f47e-4a34-4d42-9fae-f8fd520e3ffe">

## RESULT:

Thus we have successfully obtained the required result using the above-given code.
