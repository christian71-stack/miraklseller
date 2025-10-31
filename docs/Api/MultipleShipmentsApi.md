# cbdesk\Mirakl\MultipleShipmentsApi



All URIs are relative to https://your-instance.mirakl.net, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**sT01()**](MultipleShipmentsApi.md#sT01) | **POST** /api/shipments | Create shipments |
| [**sT06()**](MultipleShipmentsApi.md#sT06) | **PUT** /api/shipments/delete | Delete shipments |
| [**sT07()**](MultipleShipmentsApi.md#sT07) | **PUT** /api/shipments | Update shipment shipping origin |
| [**sT11()**](MultipleShipmentsApi.md#sT11) | **GET** /api/shipments | List shipments |
| [**sT12()**](MultipleShipmentsApi.md#sT12) | **GET** /api/shipments/items_to_ship | List items to ship |
| [**sT23()**](MultipleShipmentsApi.md#sT23) | **POST** /api/shipments/tracking | Update carrier tracking information for shipments |
| [**sT24()**](MultipleShipmentsApi.md#sT24) | **PUT** /api/shipments/ship | Validate shipments as shipped |
| [**sT26()**](MultipleShipmentsApi.md#sT26) | **PUT** /api/shipments/ready_for_pick_up | Validate shipments as ready to pick up |
| [**sT31()**](MultipleShipmentsApi.md#sT31) | **PUT** /api/shipments/additional_information | Update shipment additional information |


## `sT01()`

```php
sT01($shop_id, $st01_request): \cbdesk\Mirakl\Model\ST01Response201
```

Create shipments

Limited to 1000 shipments at a time

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new cbdesk\Mirakl\Api\MultipleShipmentsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

$associative_array = [
    'shop_id' => 56, // int | Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used.
    'st01_request' => new \cbdesk\Mirakl\Model\ST01Request(), // \cbdesk\Mirakl\Model\ST01Request
];

try {
    $result = $apiInstance->sT01($associate_array);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MultipleShipmentsApi->sT01: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Note: the input parameter is an associative array with the keys listed as the parameter names below.

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **shop_id** | **int**| Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used. | [optional] |
| **st01_request** | [**\cbdesk\Mirakl\Model\ST01Request**](../Model/ST01Request.md)|  | [optional] |

### Return type

[**\cbdesk\Mirakl\Model\ST01Response201**](../Model/ST01Response201.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `sT06()`

```php
sT06($shop_id, $st06_request): \cbdesk\Mirakl\Model\ST06Response200
```

Delete shipments

Limited to 1000 shipments at a time

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new cbdesk\Mirakl\Api\MultipleShipmentsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

$associative_array = [
    'shop_id' => 56, // int | Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used.
    'st06_request' => new \cbdesk\Mirakl\Model\ST06Request(), // \cbdesk\Mirakl\Model\ST06Request
];

try {
    $result = $apiInstance->sT06($associate_array);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MultipleShipmentsApi->sT06: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Note: the input parameter is an associative array with the keys listed as the parameter names below.

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **shop_id** | **int**| Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used. | [optional] |
| **st06_request** | [**\cbdesk\Mirakl\Model\ST06Request**](../Model/ST06Request.md)|  | [optional] |

### Return type

[**\cbdesk\Mirakl\Model\ST06Response200**](../Model/ST06Response200.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `sT07()`

```php
sT07($shop_id, $st07_request): \cbdesk\Mirakl\Model\ST07Response200
```

Update shipment shipping origin

Limited to 100 shipments at a time

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new cbdesk\Mirakl\Api\MultipleShipmentsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

$associative_array = [
    'shop_id' => 56, // int | Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used.
    'st07_request' => new \cbdesk\Mirakl\Model\ST07Request(), // \cbdesk\Mirakl\Model\ST07Request
];

try {
    $result = $apiInstance->sT07($associate_array);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MultipleShipmentsApi->sT07: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Note: the input parameter is an associative array with the keys listed as the parameter names below.

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **shop_id** | **int**| Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used. | [optional] |
| **st07_request** | [**\cbdesk\Mirakl\Model\ST07Request**](../Model/ST07Request.md)|  | [optional] |

### Return type

[**\cbdesk\Mirakl\Model\ST07Response200**](../Model/ST07Response200.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `sT11()`

```php
sT11($order_id, $shipment_state_code, $shipment_customer_debit_state_code, $last_updated_from, $last_updated_to, $shop_id, $page_token, $sort): \cbdesk\Mirakl\Model\ST11Response200
```

List shipments

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new cbdesk\Mirakl\Api\MultipleShipmentsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

$associative_array = [
    'order_id' => array('order_id_example'), // string[] | Order id for filtering. This parameter can be supplied multiple times (order_id=OR01-A&order_id=OR02-A...).
    'shipment_state_code' => array('shipment_state_code_example'), // string[] | Shipment state code for filtering. This parameter can be supplied multiple times (shipment_state_code=SHIPPING&shipment_state_code=SHIPPED...).
    'shipment_customer_debit_state_code' => array('shipment_customer_debit_state_code_example'), // string[] | Shipment customer debit state code for filtering. This parameter can be supplied multiple times (shipment_customer_debit_state_code=WAITING_TAX_CONFIRMATION&shipment_customer_debit_state_code=DEBIT_OK...).
    'last_updated_from' => new \DateTime('2013-10-20T19:20:30+01:00'), // \DateTime | Filter shipments updated after the given date.
    'last_updated_to' => new \DateTime('2013-10-20T19:20:30+01:00'), // \DateTime | Filter shipments updated before the given date.
    'shop_id' => 56, // int | Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used.
    'page_token' => 'page_token_example', // string | Token retrieved from next_page_token or previous_page_token to get to next
    'sort' => 'sort_example', // string | How the results should be sorted. Must follow \"sort=criterion,direction\" format as described in Mirakl API Documentation
];

try {
    $result = $apiInstance->sT11($associate_array);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MultipleShipmentsApi->sT11: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Note: the input parameter is an associative array with the keys listed as the parameter names below.

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **order_id** | [**string[]**](../Model/string.md)| Order id for filtering. This parameter can be supplied multiple times (order_id&#x3D;OR01-A&amp;order_id&#x3D;OR02-A...). | [optional] |
| **shipment_state_code** | [**string[]**](../Model/string.md)| Shipment state code for filtering. This parameter can be supplied multiple times (shipment_state_code&#x3D;SHIPPING&amp;shipment_state_code&#x3D;SHIPPED...). | [optional] |
| **shipment_customer_debit_state_code** | [**string[]**](../Model/string.md)| Shipment customer debit state code for filtering. This parameter can be supplied multiple times (shipment_customer_debit_state_code&#x3D;WAITING_TAX_CONFIRMATION&amp;shipment_customer_debit_state_code&#x3D;DEBIT_OK...). | [optional] |
| **last_updated_from** | **\DateTime**| Filter shipments updated after the given date. | [optional] |
| **last_updated_to** | **\DateTime**| Filter shipments updated before the given date. | [optional] |
| **shop_id** | **int**| Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used. | [optional] |
| **page_token** | **string**| Token retrieved from next_page_token or previous_page_token to get to next | [optional] |
| **sort** | **string**| How the results should be sorted. Must follow \&quot;sort&#x3D;criterion,direction\&quot; format as described in Mirakl API Documentation | [optional] |

### Return type

[**\cbdesk\Mirakl\Model\ST11Response200**](../Model/ST11Response200.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `sT12()`

```php
sT12($order_id, $fulfillment_center_code, $shipping_date_from, $shipping_date_to, $shop_id, $page_token, $sort): \cbdesk\Mirakl\Model\ST12Response200
```

List items to ship

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new cbdesk\Mirakl\Api\MultipleShipmentsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

$associative_array = [
    'order_id' => array('order_id_example'), // string[] | Order id for filtering. This parameter can be supplied multiple times (order_id=OR01-A&order_id=OR02-A...).
    'fulfillment_center_code' => array('fulfillment_center_code_example'), // string[] | Fulfillment center code for filtering. This parameter can be supplied multiple times (fulfillment_center_code=ABC&fulfillment_center_code=DEF...).
    'shipping_date_from' => new \DateTime('2013-10-20T19:20:30+01:00'), // \DateTime | Filter items that moved to shipping status after the given date.
    'shipping_date_to' => new \DateTime('2013-10-20T19:20:30+01:00'), // \DateTime | Filter items that moved to shipping status before the given date.
    'shop_id' => 56, // int | Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used.
    'page_token' => 'page_token_example', // string | Token retrieved from next_page_token or previous_page_token to get to next
    'sort' => 'sort_example', // string | How the results should be sorted. Must follow \"sort=criterion,direction\" format as described in Mirakl API Documentation
];

try {
    $result = $apiInstance->sT12($associate_array);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MultipleShipmentsApi->sT12: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Note: the input parameter is an associative array with the keys listed as the parameter names below.

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **order_id** | [**string[]**](../Model/string.md)| Order id for filtering. This parameter can be supplied multiple times (order_id&#x3D;OR01-A&amp;order_id&#x3D;OR02-A...). | [optional] |
| **fulfillment_center_code** | [**string[]**](../Model/string.md)| Fulfillment center code for filtering. This parameter can be supplied multiple times (fulfillment_center_code&#x3D;ABC&amp;fulfillment_center_code&#x3D;DEF...). | [optional] |
| **shipping_date_from** | **\DateTime**| Filter items that moved to shipping status after the given date. | [optional] |
| **shipping_date_to** | **\DateTime**| Filter items that moved to shipping status before the given date. | [optional] |
| **shop_id** | **int**| Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used. | [optional] |
| **page_token** | **string**| Token retrieved from next_page_token or previous_page_token to get to next | [optional] |
| **sort** | **string**| How the results should be sorted. Must follow \&quot;sort&#x3D;criterion,direction\&quot; format as described in Mirakl API Documentation | [optional] |

### Return type

[**\cbdesk\Mirakl\Model\ST12Response200**](../Model/ST12Response200.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `sT23()`

```php
sT23($shop_id, $st23_request): \cbdesk\Mirakl\Model\ST23Response200
```

Update carrier tracking information for shipments

If the carrier is not registered, the complete tracking url can be provided. Limited to 1000 shipments at a time.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new cbdesk\Mirakl\Api\MultipleShipmentsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

$associative_array = [
    'shop_id' => 56, // int | Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used.
    'st23_request' => new \cbdesk\Mirakl\Model\ST23Request(), // \cbdesk\Mirakl\Model\ST23Request
];

try {
    $result = $apiInstance->sT23($associate_array);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MultipleShipmentsApi->sT23: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Note: the input parameter is an associative array with the keys listed as the parameter names below.

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **shop_id** | **int**| Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used. | [optional] |
| **st23_request** | [**\cbdesk\Mirakl\Model\ST23Request**](../Model/ST23Request.md)|  | [optional] |

### Return type

[**\cbdesk\Mirakl\Model\ST23Response200**](../Model/ST23Response200.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `sT24()`

```php
sT24($shop_id, $st24_request): \cbdesk\Mirakl\Model\ST24Response200
```

Validate shipments as shipped

Limited to 1000 shipments at a time

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new cbdesk\Mirakl\Api\MultipleShipmentsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

$associative_array = [
    'shop_id' => 56, // int | Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used.
    'st24_request' => new \cbdesk\Mirakl\Model\ST24Request(), // \cbdesk\Mirakl\Model\ST24Request
];

try {
    $result = $apiInstance->sT24($associate_array);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MultipleShipmentsApi->sT24: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Note: the input parameter is an associative array with the keys listed as the parameter names below.

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **shop_id** | **int**| Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used. | [optional] |
| **st24_request** | [**\cbdesk\Mirakl\Model\ST24Request**](../Model/ST24Request.md)|  | [optional] |

### Return type

[**\cbdesk\Mirakl\Model\ST24Response200**](../Model/ST24Response200.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `sT26()`

```php
sT26($shop_id, $st26_request): \cbdesk\Mirakl\Model\ST26Response200
```

Validate shipments as ready to pick up

Limited to 1000 shipments at a time

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new cbdesk\Mirakl\Api\MultipleShipmentsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

$associative_array = [
    'shop_id' => 56, // int | Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used.
    'st26_request' => new \cbdesk\Mirakl\Model\ST26Request(), // \cbdesk\Mirakl\Model\ST26Request
];

try {
    $result = $apiInstance->sT26($associate_array);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MultipleShipmentsApi->sT26: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Note: the input parameter is an associative array with the keys listed as the parameter names below.

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **shop_id** | **int**| Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used. | [optional] |
| **st26_request** | [**\cbdesk\Mirakl\Model\ST26Request**](../Model/ST26Request.md)|  | [optional] |

### Return type

[**\cbdesk\Mirakl\Model\ST26Response200**](../Model/ST26Response200.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `sT31()`

```php
sT31($shop_id, $st31_request): \cbdesk\Mirakl\Model\ST31Response200
```

Update shipment additional information

Limited to 100 shipments at a time

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new cbdesk\Mirakl\Api\MultipleShipmentsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

$associative_array = [
    'shop_id' => 56, // int | Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used.
    'st31_request' => new \cbdesk\Mirakl\Model\ST31Request(), // \cbdesk\Mirakl\Model\ST31Request
];

try {
    $result = $apiInstance->sT31($associate_array);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MultipleShipmentsApi->sT31: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Note: the input parameter is an associative array with the keys listed as the parameter names below.

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **shop_id** | **int**| Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used. | [optional] |
| **st31_request** | [**\cbdesk\Mirakl\Model\ST31Request**](../Model/ST31Request.md)|  | [optional] |

### Return type

[**\cbdesk\Mirakl\Model\ST31Response200**](../Model/ST31Response200.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
