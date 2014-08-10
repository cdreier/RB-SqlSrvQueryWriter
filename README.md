# RB-SqlSrvQueryWriter

MSSQL / SQL-Server support plugin for the awesome RedBeanPHP ORM

---

## Dependencies

1. [RedBeanPHP](http://redbeanphp.com/)
2. [SQLSRV PHP Driver](http://www.microsoft.com/en-us/download/details.aspx?id=20098) (yes, you download an exe file which contains the dlls)

## Usage

```php
require_once 'rb.phar';
require_once 'SqlsrvQueryWriter.php';

$pdo = new PDO("sqlsrv:Server=(local)\\your_sqlserver_installation;Database=your_database_name", "username", "password");
R::setupSqlsrv($pdo);
R::freeze(false);

// just use redbeanphp
```

