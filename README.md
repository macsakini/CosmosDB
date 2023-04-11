# Azure CosmosDB

This is a wrapper around the api to make it simpler to utilize azure cosmosdb from your php services such as Wordpress, Symphony and Laravel.

Wrapper for Azure Cosmos DB.

https://learn.microsoft.com/en-us/rest/api/cosmos-db/

## Installation

Include cosmosdb/cosmosdb in your project, by adding it to your composer.json file.

```
{
    "require": {
        "cosmosdb/cosmosdb": "1.1.0"
    }
}
```

or by running

```
composer require cosmosdb/cosmosdb
```

at the root of your project.

## Usage

### Select Database

```php

$database = new Database(
    'host',
    'primary_key'
);
$response = $database->get("Variants");

```

### Delete Database

```php

$database = new Database(
    'host',
    'primary_key'
);
$response = $database->delete("Variants");

```

### List Databases

```php

$database = new Database(
    'host',
    'primary_key'
);
$response = $database->list();

```

### Create a new Database

```php

$database = new Database(
    'host',
    'primary_key'
);
$response = $database->create("Variants");

```
