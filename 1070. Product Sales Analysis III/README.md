<h2><a href="https://leetcode.com/problems/product-sales-analysis-iii">1070. Product Sales Analysis III</a></h2><h3>Medium</h3><hr><p>Table: <code>Sales</code></p>

<pre>
+-------------+-------+
| Column Name | Type  |
+-------------+-------+
| sale_id     | int   |
| product_id  | int   |
| year        | int   |
| quantity    | int   |
| price       | int   |
+-------------+-------+
(sale_id, year) is the primary key (combination of columns with unique values) of this table.
Each row records a sale of a product in a given year.
A product may have multiple sales entries in the same year.
Note that the per-unit price.
</pre>

<p>&nbsp;</p>

<p>Write a solution to find all sales that occurred in the >strong>first year</strong> each product was sold.</p>

<p>For each <code>product_id</code>, identify the earliest <code>year</code> it appears in the <code>Sales</code> table</strong>.</p>

<p>Return <strong>all</strong> sales entries for that product in that year.</p>

<p>Return a table with the following columns: <strong>product_id</strong>, <strong>first_year</strong>, <strong>quantity</strong>, and <strong>price</strong>.
Return the result in any order.</p>


<p>&nbsp;</p>
<p><strong class="example">Example 1:</strong></p>

<pre>
<strong>Input:</strong> 
Sales table:
+---------+------------+------+----------+-------+
| sale_id | product_id | year | quantity | price |
+---------+------------+------+----------+-------+ 
| 1       | 100        | 2008 | 10       | 5000  |
| 2       | 100        | 2009 | 12       | 5000  |
| 7       | 200        | 2011 | 15       | 9000  |
+---------+------------+------+----------+-------+

<strong>Output:</strong> 
+------------+------------+----------+-------+
| product_id | first_year | quantity | price |
+------------+------------+----------+-------+ 
| 100        | 2008       | 10       | 5000  |
| 200        | 2011       | 15       | 9000  |
+------------+------------+----------+-------+
