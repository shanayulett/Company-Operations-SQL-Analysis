.# Company-Operations-SQL-Analysis
SQL Analysis of Corporate departments, desk allocation, and location using a mock SQLite database

### Query 1: Desk Allocation by state
I wanted to analyze which states hold the company's largest physical footprint based on the total number of employee desks.
  Sql 
  SELECT state, SUM (num_desks) AS 
  total_desks
  FROM departments 
  GROUP BY state 
  ORDER BY total_desks desc;

  Key Insights found 

Missouri(Mo): This state is represented as the primary operational hub which has 148 desk (Maximum)
California (CA): California is mid-tier from Virginia with 89 desks (Mid-tier)
New York (NY): This state is the lowesr metric point with a total of 23 desks (Minimum)
