# SQl
SQL for PATİKA

# PATİKA 1. HOMEWORK

--SELECT title, description FROM film

--SELECT * FROM film
--WHERE length > 60 AND length < 75;

--SELECT * FROM film
--WHERE rental_rate = 0.99 AND (replacement_cost = 12.99 OR replacement_cost = 28.99);

--SELECT last_name FROM customer
--WHERE first_name = 'Mary';

--SELECT * FROM film
--WHERE length <= 50 AND rental_rate != 2.99 AND rental_rate != 4.99;

# PATİKA 2. HOMEWORK

--SELECT * FROM film
--WHERE replacement_cost BETWEEN 12.99 AND 16.99;

--SELECT first_name, last_name FROM actor
--WHERE first_name IN('Penelope','Nick','Ed');

--SELECT * FROM film
--WHERE rental_rate IN(0.99,2.99,4.99) AND replacement_cost IN(12.99,15.99,28.99);

# PATİKA 3. HOMEWORK

--SELECT country FROM country
--WHERE country LIKE 'A%a';

--SELECT country FROM country
--WHERE country LIKE '_____n';

--SELECT title FROM film
--WHERE title ILIKE '%t%t%t%t%';

--SELECT title FROM film
--WHERE title LIKE 'C%' AND length > 90 AND rental_rate = 2.99;

# PATİKA 4.HOMEWORK

--SELECT DISTINCT replacement_cost FROM film

--SELECT COUNT(DISTINCT(replacement_cost)) FROM film

--SELECT title ,rating FROM film
--WHERE title LIKE 'T%' AND rating = 'G';

--SELECT COUNT(country) FROM country
--WHERE country LIKE '_____';

--SELECT COUNT(city) FROM city
--WHERE city LIKE 'R%r';

# PATİKA 5. HOMEWORK

--SELECT title FROM film
--WHERE title LIKE '%n'
--ORDER BY length ASC
--LIMIT 5;

--SELECT title FROM film
--WHERE title LIKE '%n'
--ORDER BY length DESC
--OFFSET 5
--LIMIT 5;

--SELECT last_name FROM customer
--WHERE store_id = 1
--ORDER BY last_name DESC
--LIMIT 4;

# PATİKA 6. HOMEWORK

--SELECT AVG(rental_rate) FROM film;

--SELECT COUNT(title) FROM film
--WHERE title LIKE 'C%';

--SELECT MAX(length) FROM film
--WHERE rental_rate = 0.99;

--SELECT COUNT(replacement_cost) FROM film
--WHERE length > 150;

# PATİKA 7. HOMEWORK

--SELECT rating FROM film
--GROUP BY rating;

--SELECT replacement_cost,COUNT(replacement_cost) FROM film
--GROUP BY replacement_cost
--HAVING COUNT(replacement_cost) > 50;

--SELECT store_id,COUNT(customer) FROM customer
--GROUP BY store_id;

--SELECT country_id,COUNT(city) FROM city
--GROUP BY country_id 
--ORDER BY COUNT(city) DESC
--LIMIT 1;

# PATİKA 8. HOMEWORK

--CREATE TABLE employee(
--	id INTEGER,
--	name VARCHAR(50),
--	birthday DATE,
--	email VARCHAR(100)
--);

--insert into employee (id, name, birthday, email) 
--values (1, 'Sarette Avramovsky', '2023-03-14', 'savramovsky0@studiopress.com');

--UPDATE employee
--SET name = 'Miraç',
--	birthday = '2000-11-1',
--	email = 'senmrcc@gmail.com'
--WHERE id = 1 ;

--UPDATE employee
--SET name = 'Değiştirdim',
--	birthday = '2000-11-1',
--	email = 'değiştirim@ben.com'
--WHERE id IN(50,49,48,47);

--DELETE FROM employee
--WHERE id IN(30,31,32,33,34,35);

# PATİKA 9. HOMEWORK

--SELECT city, country FROM city
--INNER JOIN country ON city.country_id = country.country_id;

--SELECT DISTINCT payment_id, first_name, last_name FROM customer
--INNER JOIN payment ON payment.customer_id = customer.customer_id;

--SELECT rental_id, first_name, last_name FROM customer
--INNER JOIN rental ON rental.customer_id = customer.customer_id;

# PATİKA 10. HOMEWORK

--SELECT city, country FROM city
--LEFT JOIN country ON country.country_id = city.country_id;

--SELECT DISTINCT  payment_id, first_name, last_name FROM customer
--RIGHT JOIN payment ON payment.customer_id = customer.customer_id;

--SELECT rental_id, first_name, last_name FROM customer
--FULL JOIN rental ON rental.customer_id = customer.customer_id;

# PATİKA 11. HOMEWORK

--(
--	SELECT first_name FROM actor
--)
--UNION ALL
--(
--	SELECT first_name FROM customer
--);

--(
--	SELECT first_name FROM customer
--)
--INTERSECT
--(
--	SELECT first_name FROM actor
--);

--(
--	SELECT first_name FROM actor
--)
--EXCEPT
--(
--	SELECT first_name FROM customer
--);

--(
--	SELECT first_name FROM actor
--)
--UNION ALL
--(
--	SELECT first_name FROM customer
--);

--(
--	SELECT first_name FROM actor
--)
--INTERSECT ALL
--(
--	SELECT first_name FROM customer
--);

--(
--	SELECT first_name FROM actor
--)
--EXCEPT ALL
--(	
--	SELECT first_name FROM customer
--);
