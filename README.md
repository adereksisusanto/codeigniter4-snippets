# Codeigniter 4 Snippets for Vscode

This Extensions provides the Codeigniter 4 snippets

## Requirements

```bash
CodeIgniter Version : 4.1.1
```

## Install

Launch Code's command palette

```bash
ext install adereksisusanto.codeigniter4-snippets
```

### Table of Content

- [Controllers](https://github.com/adereksisusanto/codeigniter4-snippets/blob/main/docs/CONTROLLERS.md)
- [Migrations](https://github.com/adereksisusanto/codeigniter4-snippets/blob/main/docs/MIGRATIONS.md) [new]
- [Models](https://github.com/adereksisusanto/codeigniter4-snippets/blob/main/docs/MODELS.md)
- [Routes](https://github.com/adereksisusanto/codeigniter4-snippets/blob/main/docs/ROUTES.md)
- [Views](https://github.com/adereksisusanto/codeigniter4-snippets/blob/main/docs/Views.md)

### Alternate Snippets for Routes

### `[ProjectRoot]/app/Config/Routes.php`

<table>
<thead>
<tr>
<th align="center">Command</th>
<th align="center">Description</th>
<th align="center">Output</th>
</tr>
</thead>
<tbody>
<tr>
<td nowrap>ci4:routes:add</td>
<td>Make Routes add() </td>
<td>

```php
$routes->add('url', 'ControllerName::index');
```

</td>
</tr>
<!--  -->
<tr>
<td nowrap>ci4:routes:cli</td>
<td>Make Command-Line only Routes</td>
<td>

```php
$routes->cli('migrate', 'App\Database::migrate');
```

</td>
</tr>
<!--  -->
<tr>
<td nowrap>ci4:routes:env</td>
<td>Make Routes Environment</td>
<td>

```php
$routes->environment('development' , function($routes)
{
    $routes->add('builder','Tools\Builder::index');
});
```

</td>
</tr>
<!--  -->
<tr>
<td colspan="3" align="center">

[More..](https://github.com/adereksisusanto/codeigniter4-snippets/blob/main/docs/ROUTES.md)

</td>
</tr>
</tbody>
</table>

---

### Alternate Snippets for View Files

### `[ProjectRoot]/app/Views/**.php`

<table>
<thead>
<tr>
<th align="center">Command</th>
<th align="center">Description</th>
<th align="center">Output</th>
</tr>
</thead>
<tbody>
<tr>
<td nowrap>ci4:views:endSection</td>
<td>Make end Section in View files</td>
<td>

```php
<?= $this->endSection() ;?>
```

</td>
</tr>
<!--  -->
<tr>
<td nowrap>ci4:views:extend</td>
<td>Using Layouts in Views</td>
<td>

```php
<?= $this->extend('layouts') ;?>
```

</td>
</tr>
<!--  -->
<tr>
<td nowrap>ci4:views:include</td>
<td>Including View Partials</td>
<td>

```php
<?= $this->include('sidebar') ;?>
```

</td>
</tr>
<!--  -->
<tr>
<td colspan="3" align="center">

[More..](https://github.com/adereksisusanto/codeigniter4-snippets/blob/main/docs/VIEWS.md)

</td>
</tr>
</tbody>
</table>

Happy coding!

## License & Download

[![GitHub license](https://img.shields.io/github/license/adereksisusanto/codeigniter4-snippets.svg)](https://github.com/adereksisusanto/codeigniter4-snippets) ![Visual Studio Marketplace Downloads](https://img.shields.io/visual-studio-marketplace/d/adereksisusanto.codeigniter4-snippets)
