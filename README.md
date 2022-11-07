# CS20_SQLpractice
## Tasks
Write down the correct query to solve each problem – use the NORTHWIND database supplied in 
class, not the online database. 

### Part 1
<t> 1. Display the company name, contact name, and title for all CUSTOMERS. <br>
 ``` select CompanyName, ContactName, ContactTitle from customers ``` <br>
<t> 2. Display all information for all German SUPPLIERS <br>
  ``` SELECT * FROM suppliers WHERE Country = "Germany" ``` <br>
<t> 3. Display name, unit price of all PRODUCTS whose price is between $10 and $20 sorted from highest to lowest price <br>
    ``` SELECT ProductName, UnitPrice FROM products WHERE UnitPrice BETWEEN 10 AND 20 ``` <br>


### Part 2 – Advanced
You may use a manual lookup for this set of queries <br>
<t> 4. Display all countries for which the company has CUSTOMERS - with no repeats <br>
    ``` SELECT DISTINCT Country FROM customers ``` <br>
<t> 5. Display the PRODUCT name and price for suppliers 9-15 sorted by supplier number and then by product name <br>
    ``` SELECT ProductName, UnitPrice FROM products WHERE SupplierID BETWEEN 9 AND 15 ORDER BY SupplierID ASC, ProductID ASC ``` <br>
<t> 6. Display the name of all EMPLOYEES involved with sales (hint: use the title) sorted alphabetically by their last name. <br>
  ``` SELECT LastName, FirstName FROM employees WHERE Title LIKE '%Sales%' ORDER BY LastName ASC ``` <br>

### Part 3 – Joins
Use a Join to solve each of the following (i.e., you may NOT use a manual lookup) <br>
<t> 7. Display the names of all products in the beverages category <br>
    ``` ``` <br>
<t> 8. Display the product name and supplier name for all products that cost less than $10 but only for suppliers from the US. <br>
  ``` ``` <br>
