# cbdesk\Mirakl\UsersApi



All URIs are relative to https://your-instance.mirakl.net, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**rO02()**](UsersApi.md#rO02) | **GET** /api/users/shops/roles | List shop roles |


## `rO02()`

```php
rO02($shop_id): \cbdesk\Mirakl\Model\RO02Response200
```

List shop roles

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new cbdesk\Mirakl\Api\UsersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

$associative_array = [
    'shop_id' => 56, // int | Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used.
];

try {
    $result = $apiInstance->rO02($associate_array);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UsersApi->rO02: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Note: the input parameter is an associative array with the keys listed as the parameter names below.

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **shop_id** | **int**| Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used. | [optional] |

### Return type

[**\cbdesk\Mirakl\Model\RO02Response200**](../Model/RO02Response200.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
