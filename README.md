# Original https://github.com/debezium/debezium-examples/tree/main/monitoring

1. Run image
```bash
make
```
2. Run sql queries from  inventory.sql

```
mssql - localhost:1433
sa \ Password!

```

3. Start SQL Server connector
```bash
 curl -i -X POST -H "Accept:application/json" -H  "Content-Type:application/json" http://localhost:8083/connectors/ -d @register-sqlserver.json
```

4. Open a web browser and got to the Grafana UI at [http://localhost:3301](http://localhost:3000).
