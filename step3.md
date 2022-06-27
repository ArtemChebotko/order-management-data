<div class="top">

# Populate tables
### [◂](command:katapod.loadPage?step2){.steps} Step 3 of 8 [▸](command:katapod.loadPage?step4){.steps}
</div>

Execute the CQL script to insert sample data:
```
SOURCE 'assets/order_management_data.cql'
```

Retrieve all rows from table `orders_by_user`:
```
SELECT * FROM orders_by_user;        
```

Retrieve all rows from table `orders_by_id`:
```
EXPAND ON;

SELECT 
  order_id,
  item_name,
  item_id,
  item_description,
  item_price,
  item_quantity,
  order_status,
  order_timestamp,
  order_subtotal,
  order_shipping,
  order_tax,
  order_total,
  payment_summary,
  payment_details,
  billing_summary,
  billing_details,
  shipping_summary,
  shipping_details,
  delivery_id,
  delivery_details 
FROM orders_by_id;

EXPAND OFF;
```

Retrieve all rows from table `orders_by_user_item`:
```
SELECT * FROM orders_by_user_item;                    
```

Retrieve all rows from table `order_status_history_by_id`:
```
SELECT * FROM order_status_history_by_id; 
```

[continue](command:katapod.loadPage?step4){.orange_bar}