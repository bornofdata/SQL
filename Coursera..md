## 1
SELECT *
FROM dsv1069.users
WHERE deleted_at is not null

## 2
SELECT 
category, count(category)
FROM dsv1069.items group by category
