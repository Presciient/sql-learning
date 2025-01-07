
# SELECT
### Question : Find all movies with a length greater than 120 minutes.
### DATABSE : DVDRendal
For this one, I put SELECT * FROM title WHERE length > 120; because I saw "all" in the question but the best practice is to specify the collumns title and length for performance and clarity

SELECT title, length FROM film WHERE length > 120; should be preferred


![image](https://github.com/user-attachments/assets/67a33806-8387-40f4-9604-d2907b3e7e0c)
