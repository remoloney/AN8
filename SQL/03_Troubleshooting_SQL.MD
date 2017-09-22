*you are new to the department and the ask is to fix an old query that has not worked in a few years. Using the Iowa Liquor Sales Database 
See if you can fix the code.

SELECT Store, (cost –sell price),   SUM(sales), 

FROM sales

WHERE Category = ‘Tequila’

AND units purchased >2

GROUP BY Store

HAVING SUM(sales) > 30.00

ORDER BY 3
