# GROUP BY
#### Question : For each country in the customer table, calculate the number of customers and the average length of their postal codes.
#### DATABSE : Chinook

I should've named the new collumns from the aggregarated function for more clarity. I also learned the difference between specifying a collumn in the aggregarate function and not.

As we can see in the exemple, without specifying a collumn I got Chili in the results because "*" counts every row. 

If I specified the postal_code collumn, since the country Chile doesn't have one in my Data Base, it would've not appeared

I gotta be careful about wheither or not I specify a collumn depending on the results I want



![image](https://github.com/user-attachments/assets/3b98d5bd-eb67-4c66-909d-a7d0f2451173)

---

# ORDER BY
#### Question : Create a query that displays customers' last names and email addresses, sorted alphabetically by last name in ascending order, but limited to show only the first 15 results. Ensure that only active customers are included
#### DATABSE : DVDRental

This is one of the easiest function (for now). It even goes after the SELECT function in the way SQL treats commands, it's one of the last ones which makes it really easy to use

You're applying little modifications to the final cake, most of the hard work is already done. It's like only having to put the star on the Chrismast three


![image](https://github.com/user-attachments/assets/a6bc93db-95e7-46d0-8683-1e4dc3a3e0af)

---

# LIKE
#### Question : Find all products where the product name contains either 'wood' or 'metal' and has an unit that is not empty.
#### DATABSE : Northwind
The LIKE opperator is case sensitive on PostgreSQL, so I should use the UPPER() or LOWER() functions if I don't know the case of the word 
There is ILIKE for Postgre but since it only works on Postgre apparently it's not a good habit to use it. Even if it's really useful. I will stick to UPPER and LOWER for now and try to get more opinions on that

Some stuff from last lessons, targetting the right fields instead of using "*" ☑️ parentheses for AND & OR ☑️




![image](https://github.com/user-attachments/assets/65ef7f50-0195-4cfe-a707-f1299ef0f619)


---

# IN
#### Question : Using the "address" table, write a query to find all addresses that are located in one of these postal codes: '52137', '23503', '96522'.
#### DATABSE : DVDRental
It's faster than writing a bunch of ORs if there are a lot of conditions. I can also use NOT IN if needed 



![image](https://github.com/user-attachments/assets/692d7708-2566-4b8e-b7d4-f0c2a50beaa5)

---

# BETWEEN
#### Question : Using the rental table, write a query to find all rentals that occurred between '2005-07-01' and '2005-07-31' (July 2005). Display the rental_id, rental_date, and return_date columns.
#### DATABSE : DVDRental
This is an easy opperator, I should just remember that it is inclusive on both ends


![image](https://github.com/user-attachments/assets/14b49950-657d-44d9-ae32-3145c57fc5e9)

---

# AND & OR
#### Question : Find all orders that were either placed in January 2024 AND handled by employee ID 5, OR placed in December 2023 AND handled by employee ID 3.
#### DATABSE : Northwind
The parentheses are really important to combine multiple AND & OR operators. I would say that when there are two or more, I would require the parentheses. Very important

I have also specified the collums instead of using "*"


![image](https://github.com/user-attachments/assets/f9b29074-573c-4981-94ee-9fd780015430)


---


# DISTINCT
#### Question : Write a query to find all unique postal codes from the employee table.
#### DATABSE : Chinook

The DISTINCT's exercices were pretty basic. I think that it will be more complicated when I mix more keywords.



![image](https://github.com/user-attachments/assets/91a2aa9f-0f3c-4fbb-8c7c-57107dfb60d7)

------------------


# SELECT
#### Question : Find all movies with a length greater than 120 minutes.
#### DATABSE : DVDRendal

For this one, I put SELECT * FROM title WHERE length > 120; because I saw "all" in the question but the best practice is to specify the collumns title and length for performance and clarity

SELECT title, length FROM film WHERE length > 120; should be preferred


![image](https://github.com/user-attachments/assets/67a33806-8387-40f4-9604-d2907b3e7e0c)
