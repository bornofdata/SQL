## 1
SELECT *
FROM dsv1069.users
WHERE deleted_at is not null

## 2
SELECT 
category, count(category)
FROM dsv1069.items group by category

## 3
SELECT 
*
FROM dsv1069.users as u

right JOIN dsv1069.orders as o
on
u.id = o.user_id

## 4
