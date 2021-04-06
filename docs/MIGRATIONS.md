# Alternate Snippets for Migrations

## `[ProjectRoot]/app/Database/Migrations/`

# Table of Content

- [Create Migration](#create-migration) [new]
  - [Migration Up](#migration-up) [new]
  - [Migration Down](#migration-down) [new]
- [Create Table](#create-table) [new]
  - [Timestamp](#timestamp) [new]

## Create Migration

**Command**

```bash
ci4:migration
```

**Output**

```php
<?php

namespace App\Database\Migrations;

use CodeIgniter\Database\Migration;

class AddBlog extends Migration
{
    public function up()
    {
        //
    }

    public function down()
    {
        //
    }
}
```

- ### Migration Up

  **Command**

  ```bash
  ci4:migration:up
  ```

  **Output**

  ```php
  public function up()
  {
    $this->forge->addField([
        'id' => [
            'type' => 'INT',
            'constraint' => 11,
            'unsigned' => true,
            'auto_increment' => true,
        ],
        'name' => [
            'type' => 'VARCHAR',
            'constraint' => 255,
        ],
        'created_at' => [
            'type' => 'DATETIME',
            'null' => true,
        ],
        'updated_at' => [
            'type' => 'DATETIME',
            'null' => true,
        ],
        'deleted_at' => [
            'type' => 'DATETIME',
            'null' => true,
        ],
    ]);
    $this->forge->addKey('id', true);
    $this->forge->createTable('tableName');
  }
  ```

- ### Migration Down

  **Command**

  ```bash
  ci4:migration:down
  ```

  **Output**

  ```php
  public function down()
  {
    $this->forge->dropTable('tableName');
  }
  ```

## Create Table

- ### Timestamp

  **Command :**

  ```bash
  ci4:migration:timestamp
  ```

  **Output :**

  ```php
  'created_at' => [
    'type' => 'DATETIME',
    'null' => true,
  ],
  'updated_at' => [
    'type' => 'DATETIME',
    'null' => true,
  ],
  'deleted_at' => [
    'type' => 'DATETIME',
    'null' => true,
  ],
  ```
