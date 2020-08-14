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
SELECT 
COUNT(event_id) AS events
FROM dsv1069.events
WHERE event_name LIKE '%view%'

## 5 
SELECT 
count(distinct i.id)
FROM dsv1069.items as i
inner JOIN
dsv1069.orders as o
on
i.id = o.item_id
WHERE o.paid_at is not null

## 6 
select 
users.id, min(orders.paid_at)
FROM
dsv1069.orders
full OUTER JOIN
dsv1069.users
on 
orders.user_id = users.id
where orders.paid_at IS NOT NULL
GROUP BY users.id

## 7
