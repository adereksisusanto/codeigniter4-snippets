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
<td nowrap>ci4:routes:get</td>
<td>Make Routes get()</td>
<td>

```php
$routes->get('url', 'ControllerName::index');
```

</td>
</tr>
<!--  -->
<tr>
<td nowrap>ci4:routes:group</td>
<td>Make Routes group()</td>
<td>

```php
$routes->group('admin', function($routes)
{
    //Route
});
```

</td>
</tr>
<!--  -->
<tr>
<td nowrap>ci4:routes:group-filter</td>
<td>Make Routes group() filter</td>
<td>

```php
$routes->group('api' , ['filter' => 'api-auth'], function($routes)
{
    $routes->resource('url');
});
```

</td>
</tr>
<!--  -->
<tr>
<td nowrap>ci4:routes:group-multiple</td>
<td>Make Routes group() multiple</td>
<td>

```php
$routes->group('admin', function($routes)
{
    $routes->group('users', function($routes)
    {
        //Route
    });
});
```

</td>
</tr>
<!--  -->
<tr>
<td nowrap>ci4:routes:group-namespace</td>
<td>Make Routes group() namespace</td>
<td>

```php
$routes->group('api' , ['namespace' => 'App\API\v1'], function($routes)
{
    //Route
});
```

</td>
</tr>
<!--  -->
<tr>
<td nowrap>ci4:routes:post</td>
<td>Make Routes post()</td>
<td>

```php
$routes->post('url', 'ControllerName::index');
```

</td>
</tr>
<!--  -->
<tr>
<td nowrap>ci4:routes:subdomain</td>
<td>Make Routes Limit to Subdomains</td>
<td>

```php
$routes->add('from', 'to', ['subdomain' => '*']);
```

</td>
</tr>
<!--  -->
</tbody>
</table>
