<div class="top">

# Create a keyspace
### [◂](command:katapod.loadPage?intro){.steps} Step 1 of 8 [▸](command:katapod.loadPage?step2){.steps}
</div>

Start the CQL shell:
```
cqlsh
```

Create the `order_management_data` keyspace:
```
CREATE KEYSPACE order_management_data
WITH replication = {
  'class': 'NetworkTopologyStrategy', 
  'DC-Houston': 1 };
```

Set the current working keyspace:
```
USE order_management_data;
```

[continue](command:katapod.loadPage?step2){.orange_bar}