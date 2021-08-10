
# Helpful Queries (SQLServer)
#### Select Top N rows from table
```
Select Top(5) * from dbo.TABLE_NAME
```

#### Get # of rows in table
```
Select Count(*) from dbo.TABLE_NAME
```

#### Select based on WHERE clause
```
Select * from dbo.TABLE_NAME
WHERE symbol="hello_world"
```

#### Select using an ORDER BY clause
```
Select * from dbo.Currencies
Order by date desc
```


#### Delete all rows older than N days
```
DELETE FROM dbo.TABLE_NAME
WHERE date < DATEADD(dd,-N,GETDATE());
```

#### Delete all rows older than N hours
```
DELETE FROM dbo.TABLE_NAME
WHERE date < DATEADD(hh,-N,GETDATE());
```