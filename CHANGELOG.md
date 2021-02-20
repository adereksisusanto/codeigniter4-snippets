# Change Log

All notable changes to the "codeigniter4-snippets" extension will be documented in this file.

Check [Keep a Changelog](https://github.com/adereksisusanto/codeigniter4-snippets/releases/tag/0.0.3) for recommendations on how to structure this file.

## [Released - 0.0.3]

- #### Fixed Bugs
- #### Add Snippets

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
<td>ci4_routes_add</td>
<td>Make <b>routes add</b></td>
<td>

```php
$routes->add('url', 'ControllerName::index');
```

</td>
</tr>
<tr>
<td>ci4_routes_cli</td>
<td>Make <b>Command-Line only Routes</b></td>
<td>

```php
$routes->cli('migrate', 'App\Database::migrate');
```

</td>
</tr>
<tr>
<td>ci4_routes_env</td>
<td>Make <b>routes environment</b></td>
<td>

```php
$routes->environment('development' , function($routes)
{
    $routes->add('builder','Tools\Builder::index');
});
```

</td>
</tr>
<tr>
<td>ci4_routes_get</td>
<td>Make <b>routes get</b></td>
<td>

```php
$routes->get('url', 'ControllerName::index');
```

</td>
</tr>
<tr>
<td>ci4_routes_group</td>
<td>Make <b>routes group</b></td>
<td>

```php
$routes->group('admin', function($routes)
{
    $routes->add('url','ControllerName::index');
});
```

</td>
</tr>
<tr>
<td>ci4_routes_group_filter</td>
<td>Make <b>routes group filter</b></td>
<td>

```php
$routes->group('api' , ['filter' => 'api-auth'], function($routes)
{
    $routes->resource('url');
});
```

</td>
</tr>
<tr>
<td>ci4_routes_group_multiple</td>
<td>Make <b>routes group multiple</b></td>
<td>

```php
$routes->group('admin', function($routes)
{
    $routes->group('users', function($routes)
    {
        $routes->add('list','Admin\Users::list');
    });
});
```

</td>
</tr>
<tr>
<td>ci4_routes_group_namespace</td>
<td>Make <b>routes group namespace</b></td>
<td>

```php
$routes->group('api' , ['namespace' => 'App\API\v1'], function($routes)
{
    $routes->resource('url');
});
```

</td>
</tr>
<tr>
<td>ci4_routes_post</td>
<td>Make <b>routes post</b></td>
<td>

```php
$routes->post('url', 'ControllerName::index');
```

</td>
</tr>
<tr>
<td>ci4_routes_subdomain</td>
<td>Make <b>Routes Limit to Subdomains</b></td>
<td>

```php
$routes->add('from', 'to', ['subdomain' => '*']);
```

</td>
</tr>
<tr>
<td>ci4_routes_verbs</td>
<td>HTTP verbs in routes, HTTP verb (<b>GET, POST, PUT, DELETE, etc</b>)</td>
<td>

```php
$routes->get('products', 'Product::feature');
or
$routes->post('products', 'Product::feature');
or
$routes->put('products/(:num)', 'Product::feature');
or
$routes->delete('products/(:num)', 'Product::feature');
```

</td>
</tr>
</tbody>
</table>

## License & Download

[![GitHub license](https://img.shields.io/github/license/adereksisusanto/codeigniter4-snippets.svg)](https://github.com/adereksisusanto/codeigniter4-snippets) ![Visual Studio Marketplace Downloads](https://img.shields.io/visual-studio-marketplace/d/adereksisusanto.codeigniter4-snippets)
