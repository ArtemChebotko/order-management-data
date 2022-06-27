<div class="top">

# Design query Q3
### [◂](command:katapod.loadPage?step5){.steps} Step 6 of 8 [▸](command:katapod.loadPage?step7){.steps}
</div>

Find all orders that contain item `n-0023` and are placed by user `joe`; sort by order timestamp (desc):

<details>
  <summary>Solution</summary>

```
SELECT * 
FROM orders_by_user_item
WHERE item_id = 'n-0023'
  AND user_id = 'joe';  
```

</details>

[continue](command:katapod.loadPage?step7){.orange_bar}