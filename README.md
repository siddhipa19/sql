USE sql_store;

SELECT * FROM customers;

SELECT first_name , last_name FROM customers;

SELECT last_name , first_name , points , points + 10 AS 'discount factor' FROM customers;	

--DISTINCT;

SELECT DISTINCT state FROM customers;

--return all the products , name , unit price , new price (unit price *1.1);

SELECT name , unit_price, unit_price * 1.1 AS 'new price' FROM products;

--where clause;

SELECT * FROM customers WHERE points > 3000;

SELECT * FROM customers WHERE state = 'VA' AND points > 1000;

SELECT * FROM customers WHERE state <> 'VA';

SELECT *FROM customers WHERE state <> ' va' AND points > 1000;

SELECT * FROM customers WHERE birth_date > '1980-01-01';

--orders placed this year;

SELECT * FROM orders WHERE order_date > '2017-12-31';

git push
