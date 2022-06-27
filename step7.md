<div class="top">

# Design query Q4
### [◂](command:katapod.loadPage?step6){.steps} Step 7 of 8 [▸](command:katapod.loadPage?step8){.steps}
</div>

Find a status history for order `111-0461064-1669732`; sort by status timestamp (desc):

<details>
  <summary>Solution</summary>

```
SELECT * 
FROM order_status_history_by_id
WHERE order_id = '111-0461064-1669732'; 
```

</details>

[continue](command:katapod.loadPage?step8){.orange_bar}
