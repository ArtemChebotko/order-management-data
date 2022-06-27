<div class="top">

# Design query Q2
### [◂](command:katapod.loadPage?step4){.steps} Step 5 of 8 [▸](command:katapod.loadPage?step6){.steps}
</div>

Find all information about order `113-3827060-8722206`; sort items by name (asc):
 
<details>
  <summary>Solution</summary>

```
EXPAND ON;

SELECT * 
FROM orders_by_id
WHERE order_id = '113-3827060-8722206';

EXPAND OFF;
```

</details>

[continue](command:katapod.loadPage?step6){.orange_bar}