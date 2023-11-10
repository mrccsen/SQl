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
