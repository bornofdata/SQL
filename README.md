# SQL
SQL Projects


Note: When querying a table, remember to prepend dsv1069, which is the schema, or folder
that contains the course data.
## Exercise 1:
Goal: Here we use users table to pull a list of user email addresses. Edit the query to pull email
addresses, but only for non-deleted users.
### Starter Code:
SELECT *
FROM dsv1069.users
## Exercise 2:
--Goal: Use the items table to count the number of items for sale in each category
Starter Code: (none)
## Exercise 3:
--Goal: Select all of the columns from the result when you JOIN the users table to the orders
table
Starter Code: (none)
## Exercise 4:
--Goal: Check out the query below. This is not the right way to count the number of viewed_item
events. Determine what is wrong and correct the error.
### Starter Code:
SELECT
COUNT(event_id) AS events
FROM dsv1069.events
WHERE event_name = ‘view_item’
## Exercise 5:
--Goal:Compute the number of items in the items table which have been ordered. The query
below runs, but it isn’t right. Determine what is wrong and correct the error or start from scratch.
Starter Code:
--Error: This query runs but the number isn’t right
## Exercise 6:
--Goal: For each user figure out IF a user has ordered something, and when their first purchase
was. The query below doesn’t return info for any of the users who haven’t ordered anything.
Starter Code:
## Exercise 7:
--Goal: Figure out what percent of users have ever viewed the user profile page, but this query
isn’t right. Check to make sure the number of users adds up, and if not, fix the query.
Starter Code:
