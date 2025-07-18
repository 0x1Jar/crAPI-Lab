```
curl --location 'http://localhost:8888/workshop/api/shop/orders' \
--header 'Content-Type: application/json' \
--header 'Authorization: Bearer YOUR_ACTUAL_TOKEN' \
--data-raw '{
    "product_id": 2,
    "quantity": -1,
}'
```