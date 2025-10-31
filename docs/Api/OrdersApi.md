# cbdesk\Mirakl\OrdersApi



All URIs are relative to https://your-instance.mirakl.net, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**oR04()**](OrdersApi.md#oR04) | **PUT** /api/orders | Patch update orders |
| [**oR07()**](OrdersApi.md#oR07) | **PUT** /api/orders/shipping_from | Update order line shipping origin |
| [**oR11()**](OrdersApi.md#oR11) | **GET** /api/orders | List orders with pagination |
| [**oR13()**](OrdersApi.md#oR13) | **POST** /api/orders/async-export | Export orders asynchronously |
| [**oR14()**](OrdersApi.md#oR14) | **GET** /api/orders/async-export/status/{tracking_id} | Get the status of an asynchronous order export. |
| [**oR21()**](OrdersApi.md#oR21) | **PUT** /api/orders/{order_id}/accept | Accept or refuse order lines |
| [**oR23()**](OrdersApi.md#oR23) | **PUT** /api/orders/{order_id}/tracking | Update carrier tracking information for a specific order |
| [**oR24()**](OrdersApi.md#oR24) | **PUT** /api/orders/{order_id}/ship | Validate the shipment of an order |
| [**oR28()**](OrdersApi.md#oR28) | **PUT** /api/orders/refund | Perform refunds on order lines |
| [**oR29()**](OrdersApi.md#oR29) | **PUT** /api/orders/{order_id}/cancel | Perform a full cancelation of an order |
| [**oR30()**](OrdersApi.md#oR30) | **PUT** /api/orders/cancel | Perform cancelations on order lines |
| [**oR31()**](OrdersApi.md#oR31) | **PUT** /api/orders/{order_id}/additional_fields | Update the custom fields of an order and its order lines |
| [**oR32()**](OrdersApi.md#oR32) | **PUT** /api/orders/adjust | Adjust order line |
| [**oR51()**](OrdersApi.md#oR51) | **GET** /api/orders/{order_id}/evaluation | Get the evaluation of an order |
| [**oR72()**](OrdersApi.md#oR72) | **GET** /api/orders/documents | Lists order&#39;s documents |
| [**oR73()**](OrdersApi.md#oR73) | **GET** /api/orders/documents/download | Download one or multiple documents attached to one or multiple orders |
| [**oR75()**](OrdersApi.md#oR75) | **GET** /api/orders/taxes | List all the order taxes available on the platform |
| [**oR76()**](OrdersApi.md#oR76) | **DELETE** /api/orders/documents/{document_id} | Delete an order document |


## `oR04()`

```php
oR04($shop_id, $or04_request): \cbdesk\Mirakl\Model\OR04Response200
```

Patch update orders

<p>Update orders information field by field: unspecified fields will not be updated. To remove the value for a field, send it with the 'null' value (not allowed for the required fields).</p><p>You cannot use API OR04 to update customer-related information if the customer has been anonymized via API AN01.</p><p><span class='red'>A maximum of 100 orders can be sent at once.</span></p>

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new cbdesk\Mirakl\Api\OrdersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

$associative_array = [
    'shop_id' => 56, // int | Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used.
    'or04_request' => new \cbdesk\Mirakl\Model\OR04Request(), // \cbdesk\Mirakl\Model\OR04Request
];

try {
    $result = $apiInstance->oR04($associate_array);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling OrdersApi->oR04: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Note: the input parameter is an associative array with the keys listed as the parameter names below.

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **shop_id** | **int**| Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used. | [optional] |
| **or04_request** | [**\cbdesk\Mirakl\Model\OR04Request**](../Model/OR04Request.md)|  | [optional] |

### Return type

[**\cbdesk\Mirakl\Model\OR04Response200**](../Model/OR04Response200.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `oR07()`

```php
oR07($shop_id, $or07_request): \cbdesk\Mirakl\Model\OR07Response200
```

Update order line shipping origin

<p>Update shipping origin (<code>shipping_from</code>) information on order lines.</p> <p><span class='red'>A maximum of 100 order lines can be sent at once.</span></p>

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new cbdesk\Mirakl\Api\OrdersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

$associative_array = [
    'shop_id' => 56, // int | Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used.
    'or07_request' => new \cbdesk\Mirakl\Model\OR07Request(), // \cbdesk\Mirakl\Model\OR07Request
];

try {
    $result = $apiInstance->oR07($associate_array);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling OrdersApi->oR07: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Note: the input parameter is an associative array with the keys listed as the parameter names below.

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **shop_id** | **int**| Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used. | [optional] |
| **or07_request** | [**\cbdesk\Mirakl\Model\OR07Request**](../Model/OR07Request.md)|  | [optional] |

### Return type

[**\cbdesk\Mirakl\Model\OR07Response200**](../Model/OR07Response200.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `oR11()`

```php
oR11($order_ids, $order_references_for_customer, $order_references_for_seller, $order_state_codes, $channel_codes, $only_null_channel, $start_date, $end_date, $start_update_date, $end_update_date, $customer_debited, $payment_workflow, $has_incident, $fulfillment_center_code, $order_tax_mode, $shop_id, $locale, $max, $offset, $sort, $order): \cbdesk\Mirakl\Model\OR11Response200
```

List orders with pagination

Pagination is enabled by default. For large requests, use asynchronous order export APIs OR13, OR14 and OR15 instead.<br/>

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new cbdesk\Mirakl\Api\OrdersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

$associative_array = [
    'order_ids' => 'order_ids_example', // string | A comma-separated list of order's identifiers
    'order_references_for_customer' => 'order_references_for_customer_example', // string | A comma-separated list of order references for customer
    'order_references_for_seller' => 'order_references_for_seller_example', // string | A comma-separated list of order references for seller
    'order_state_codes' => 'order_state_codes_example', // string | A comma-separated list of order state's codes
    'channel_codes' => 'channel_codes_example', // string | A comma-separated list of channel codes
    'only_null_channel' => false, // bool | Return only orders without channel. If <code>true</code>, ignore the <code>channel_codes</code>
    'start_date' => new \DateTime('2013-10-20T19:20:30+01:00'), // \DateTime | Start creation date for filtering
    'end_date' => new \DateTime('2013-10-20T19:20:30+01:00'), // \DateTime | End creation date for filtering
    'start_update_date' => new \DateTime('2013-10-20T19:20:30+01:00'), // \DateTime | Start update date for filtering. Mirakl will subtract a time delta to ensure no orders are missed due to network and/or software latency.
    'end_update_date' => new \DateTime('2013-10-20T19:20:30+01:00'), // \DateTime | End update date for filtering
    'customer_debited' => True, // bool | Order paid by customer
    'payment_workflow' => 'payment_workflow_example', // string | Payment workflow of an order
    'has_incident' => True, // bool | If <code>true</code> returns only orders with incidents in progress, if <code>false</code> returns orders without incidents in progress. If not provided, all orders with or without incident will be returned
    'fulfillment_center_code' => array('fulfillment_center_code_example'), // string[] | Code of the fulfillment center
    'order_tax_mode' => 'order_tax_mode_example', // string | Please note: If the taxes are not specified, the prices with mode TAX_EXCLUDED and with mode TAX_INCLUDED will return the same amounts.<br>Possible values:<ul><li><code>TAX_EXCLUDED</code>: the price fields (price, unit price, shipping price, cancellation amount, refund amount and order total prices) do not include taxes.</li><li><code>TAX_INCLUDED</code>: the price fields include the tax amount. </li></ul><li>If this query parameter is not specified, the default order tax mode of the platform is used.</li>
    'shop_id' => 56, // int | Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used.
    'locale' => 'locale_example', // string | &lt;ISO-639&gt;_&lt;ISO-3166&gt; (\"en_US\") or &lt;ISO-639&gt; (\"en\") locale for internationalized data translation. The APIs only accept locales that are equivalent to the languages activated in the back-office.
    'max' => 56, // int | Maximum number of items returned per page
    'offset' => 56, // int | Index of the first item (among all the results) in the returned page
    'sort' => 'sort_example', // string | How the results should be sorted
    'order' => 'order_example', // string | Sort direction
];

try {
    $result = $apiInstance->oR11($associate_array);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling OrdersApi->oR11: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Note: the input parameter is an associative array with the keys listed as the parameter names below.

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **order_ids** | **string**| A comma-separated list of order&#39;s identifiers | [optional] |
| **order_references_for_customer** | **string**| A comma-separated list of order references for customer | [optional] |
| **order_references_for_seller** | **string**| A comma-separated list of order references for seller | [optional] |
| **order_state_codes** | **string**| A comma-separated list of order state&#39;s codes | [optional] |
| **channel_codes** | **string**| A comma-separated list of channel codes | [optional] |
| **only_null_channel** | **bool**| Return only orders without channel. If &lt;code&gt;true&lt;/code&gt;, ignore the &lt;code&gt;channel_codes&lt;/code&gt; | [optional] [default to false] |
| **start_date** | **\DateTime**| Start creation date for filtering | [optional] |
| **end_date** | **\DateTime**| End creation date for filtering | [optional] |
| **start_update_date** | **\DateTime**| Start update date for filtering. Mirakl will subtract a time delta to ensure no orders are missed due to network and/or software latency. | [optional] |
| **end_update_date** | **\DateTime**| End update date for filtering | [optional] |
| **customer_debited** | **bool**| Order paid by customer | [optional] |
| **payment_workflow** | **string**| Payment workflow of an order | [optional] |
| **has_incident** | **bool**| If &lt;code&gt;true&lt;/code&gt; returns only orders with incidents in progress, if &lt;code&gt;false&lt;/code&gt; returns orders without incidents in progress. If not provided, all orders with or without incident will be returned | [optional] |
| **fulfillment_center_code** | [**string[]**](../Model/string.md)| Code of the fulfillment center | [optional] |
| **order_tax_mode** | **string**| Please note: If the taxes are not specified, the prices with mode TAX_EXCLUDED and with mode TAX_INCLUDED will return the same amounts.&lt;br&gt;Possible values:&lt;ul&gt;&lt;li&gt;&lt;code&gt;TAX_EXCLUDED&lt;/code&gt;: the price fields (price, unit price, shipping price, cancellation amount, refund amount and order total prices) do not include taxes.&lt;/li&gt;&lt;li&gt;&lt;code&gt;TAX_INCLUDED&lt;/code&gt;: the price fields include the tax amount. &lt;/li&gt;&lt;/ul&gt;&lt;li&gt;If this query parameter is not specified, the default order tax mode of the platform is used.&lt;/li&gt; | [optional] |
| **shop_id** | **int**| Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used. | [optional] |
| **locale** | **string**| &amp;lt;ISO-639&amp;gt;_&amp;lt;ISO-3166&amp;gt; (\&quot;en_US\&quot;) or &amp;lt;ISO-639&amp;gt; (\&quot;en\&quot;) locale for internationalized data translation. The APIs only accept locales that are equivalent to the languages activated in the back-office. | [optional] |
| **max** | **int**| Maximum number of items returned per page | [optional] |
| **offset** | **int**| Index of the first item (among all the results) in the returned page | [optional] |
| **sort** | **string**| How the results should be sorted | [optional] |
| **order** | **string**| Sort direction | [optional] |

### Return type

[**\cbdesk\Mirakl\Model\OR11Response200**](../Model/OR11Response200.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `oR13()`

```php
oR13($shop_id, $locale, $or13_request): \cbdesk\Mirakl\Model\OR13Response200
```

Export orders asynchronously

<p>The API returns a tracking id to be used to query API OR14.<br />Mirakl recommends to use API OR13 instead of API OR11 as it can handle very large volumes of data.<br />You must give at least one date range filter: created or last updated date.<br />API OR13 supports the chunk of the export file into multiple files in order to:</p><ul><li>respect a maximum megabyte weight using the <code>megabytes_per_chunk</code> parameter.</li><li>respect a maximum amount of exported items using the <code>items_per_chunk</code> parameter.</li></ul><br />Only one export request can be created for the same shop account.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new cbdesk\Mirakl\Api\OrdersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

$associative_array = [
    'shop_id' => 56, // int | Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used.
    'locale' => 'locale_example', // string | &lt;ISO-639&gt;_&lt;ISO-3166&gt; (\"en_US\") or &lt;ISO-639&gt; (\"en\") locale for internationalized data translation. The APIs only accept locales that are equivalent to the languages activated in the back-office.
    'or13_request' => new \cbdesk\Mirakl\Model\OR13Request(), // \cbdesk\Mirakl\Model\OR13Request
];

try {
    $result = $apiInstance->oR13($associate_array);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling OrdersApi->oR13: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Note: the input parameter is an associative array with the keys listed as the parameter names below.

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **shop_id** | **int**| Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used. | [optional] |
| **locale** | **string**| &amp;lt;ISO-639&amp;gt;_&amp;lt;ISO-3166&amp;gt; (\&quot;en_US\&quot;) or &amp;lt;ISO-639&amp;gt; (\&quot;en\&quot;) locale for internationalized data translation. The APIs only accept locales that are equivalent to the languages activated in the back-office. | [optional] |
| **or13_request** | [**\cbdesk\Mirakl\Model\OR13Request**](../Model/OR13Request.md)|  | [optional] |

### Return type

[**\cbdesk\Mirakl\Model\OR13Response200**](../Model/OR13Response200.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `oR14()`

```php
oR14($tracking_id, $shop_id): \cbdesk\Mirakl\Model\OR14Response200
```

Get the status of an asynchronous order export.

<p>Use this API to query the order export status after an API OR13 call.<br />Until the export via API OR13 is complete, the status returned by API OR14 is <code>PENDING</code>.<br />You must call API OR14 until you get the <code>COMPLETED</code> status which correspond to a completed and successful export from API OR13.<br />The URLs in API OR14 response contain all the files from API OR13 export.<br />Browse those urls and query them using the GET method.<br />In case of error, the status is <code>FAILED</code>.<br />In case of export canceled, the status is <code>CANCELED</code>.<br /></p>

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new cbdesk\Mirakl\Api\OrdersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

$associative_array = [
    'tracking_id' => 'tracking_id_example', // string | Id of the previously created asynchronous order export
    'shop_id' => 56, // int | Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used.
];

try {
    $result = $apiInstance->oR14($associate_array);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling OrdersApi->oR14: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Note: the input parameter is an associative array with the keys listed as the parameter names below.

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **tracking_id** | **string**| Id of the previously created asynchronous order export | |
| **shop_id** | **int**| Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used. | [optional] |

### Return type

[**\cbdesk\Mirakl\Model\OR14Response200**](../Model/OR14Response200.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `oR21()`

```php
oR21($order_id, $shop_id, $or21_request)
```

Accept or refuse order lines

Accept or refuse order lines in the <code>WAITING_ACCEPTANCE</code> status

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new cbdesk\Mirakl\Api\OrdersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

$associative_array = [
    'order_id' => 'order_id_example', // string | Order's identifier
    'shop_id' => 56, // int | Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used.
    'or21_request' => new \cbdesk\Mirakl\Model\OR21Request(), // \cbdesk\Mirakl\Model\OR21Request
];

try {
    $apiInstance->oR21($associate_array);
} catch (Exception $e) {
    echo 'Exception when calling OrdersApi->oR21: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Note: the input parameter is an associative array with the keys listed as the parameter names below.

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **order_id** | **string**| Order&#39;s identifier | |
| **shop_id** | **int**| Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used. | [optional] |
| **or21_request** | [**\cbdesk\Mirakl\Model\OR21Request**](../Model/OR21Request.md)|  | [optional] |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `oR23()`

```php
oR23($order_id, $shop_id, $or23_request)
```

Update carrier tracking information for a specific order

If the carrier is not registered, the complete tracking url can be provided.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new cbdesk\Mirakl\Api\OrdersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

$associative_array = [
    'order_id' => 'order_id_example', // string | Order identifier
    'shop_id' => 56, // int | Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used.
    'or23_request' => new \cbdesk\Mirakl\Model\OR23Request(), // \cbdesk\Mirakl\Model\OR23Request
];

try {
    $apiInstance->oR23($associate_array);
} catch (Exception $e) {
    echo 'Exception when calling OrdersApi->oR23: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Note: the input parameter is an associative array with the keys listed as the parameter names below.

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **order_id** | **string**| Order identifier | |
| **shop_id** | **int**| Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used. | [optional] |
| **or23_request** | [**\cbdesk\Mirakl\Model\OR23Request**](../Model/OR23Request.md)|  | [optional] |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `oR24()`

```php
oR24($order_id, $shop_id)
```

Validate the shipment of an order

Validate the shipment of an order in the <code>SHIPPING</code> status

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new cbdesk\Mirakl\Api\OrdersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

$associative_array = [
    'order_id' => 'order_id_example', // string | Order's identifier
    'shop_id' => 56, // int | Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used.
];

try {
    $apiInstance->oR24($associate_array);
} catch (Exception $e) {
    echo 'Exception when calling OrdersApi->oR24: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Note: the input parameter is an associative array with the keys listed as the parameter names below.

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **order_id** | **string**| Order&#39;s identifier | |
| **shop_id** | **int**| Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used. | [optional] |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `oR28()`

```php
oR28($shop_id, $or28_request): \cbdesk\Mirakl\Model\OR28Response200
```

Perform refunds on order lines

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new cbdesk\Mirakl\Api\OrdersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

$associative_array = [
    'shop_id' => 56, // int | Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used.
    'or28_request' => new \cbdesk\Mirakl\Model\OR28Request(), // \cbdesk\Mirakl\Model\OR28Request
];

try {
    $result = $apiInstance->oR28($associate_array);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling OrdersApi->oR28: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Note: the input parameter is an associative array with the keys listed as the parameter names below.

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **shop_id** | **int**| Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used. | [optional] |
| **or28_request** | [**\cbdesk\Mirakl\Model\OR28Request**](../Model/OR28Request.md)|  | [optional] |

### Return type

[**\cbdesk\Mirakl\Model\OR28Response200**](../Model/OR28Response200.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `oR29()`

```php
oR29($order_id, $shop_id)
```

Perform a full cancelation of an order

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new cbdesk\Mirakl\Api\OrdersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

$associative_array = [
    'order_id' => 'order_id_example', // string | Order's identifier
    'shop_id' => 56, // int | Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used.
];

try {
    $apiInstance->oR29($associate_array);
} catch (Exception $e) {
    echo 'Exception when calling OrdersApi->oR29: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Note: the input parameter is an associative array with the keys listed as the parameter names below.

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **order_id** | **string**| Order&#39;s identifier | |
| **shop_id** | **int**| Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used. | [optional] |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `oR30()`

```php
oR30($shop_id, $or30_request): \cbdesk\Mirakl\Model\OR30Response200
```

Perform cancelations on order lines

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new cbdesk\Mirakl\Api\OrdersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

$associative_array = [
    'shop_id' => 56, // int | Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used.
    'or30_request' => new \cbdesk\Mirakl\Model\OR30Request(), // \cbdesk\Mirakl\Model\OR30Request
];

try {
    $result = $apiInstance->oR30($associate_array);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling OrdersApi->oR30: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Note: the input parameter is an associative array with the keys listed as the parameter names below.

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **shop_id** | **int**| Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used. | [optional] |
| **or30_request** | [**\cbdesk\Mirakl\Model\OR30Request**](../Model/OR30Request.md)|  | [optional] |

### Return type

[**\cbdesk\Mirakl\Model\OR30Response200**](../Model/OR30Response200.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `oR31()`

```php
oR31($order_id, $shop_id, $or31_request): \cbdesk\Mirakl\Model\OR31Response200
```

Update the custom fields of an order and its order lines

Only specified custom field values will be updated.<br/>In order to delete an custom field's value, set it to null or an empty string. Note that you may not delete the value of a required custom field value.<br/>Output will return information on the status of the update attempt by giving:<ul>    <li>either all of the order and its order lines custom field values after the update</li>    <li>or in case of errors, the list of errors and the body of the initial call</li></ul>

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new cbdesk\Mirakl\Api\OrdersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

$associative_array = [
    'order_id' => 'order_id_example', // string | Order identifier
    'shop_id' => 56, // int | Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used.
    'or31_request' => new \cbdesk\Mirakl\Model\OR31Request(), // \cbdesk\Mirakl\Model\OR31Request
];

try {
    $result = $apiInstance->oR31($associate_array);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling OrdersApi->oR31: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Note: the input parameter is an associative array with the keys listed as the parameter names below.

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **order_id** | **string**| Order identifier | |
| **shop_id** | **int**| Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used. | [optional] |
| **or31_request** | [**\cbdesk\Mirakl\Model\OR31Request**](../Model/OR31Request.md)|  | [optional] |

### Return type

[**\cbdesk\Mirakl\Model\OR31Response200**](../Model/OR31Response200.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `oR32()`

```php
oR32($shop_id, $or32_request): \cbdesk\Mirakl\Model\OR32Response200
```

Adjust order line

<p>Update order line actual measurement: it will create a refund or cancelation associated to the order line. </p>

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new cbdesk\Mirakl\Api\OrdersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

$associative_array = [
    'shop_id' => 56, // int | Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used.
    'or32_request' => new \cbdesk\Mirakl\Model\OR32Request(), // \cbdesk\Mirakl\Model\OR32Request
];

try {
    $result = $apiInstance->oR32($associate_array);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling OrdersApi->oR32: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Note: the input parameter is an associative array with the keys listed as the parameter names below.

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **shop_id** | **int**| Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used. | [optional] |
| **or32_request** | [**\cbdesk\Mirakl\Model\OR32Request**](../Model/OR32Request.md)|  | [optional] |

### Return type

[**\cbdesk\Mirakl\Model\OR32Response200**](../Model/OR32Response200.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `oR51()`

```php
oR51($order_id, $shop_id, $locale): \cbdesk\Mirakl\Model\OR51Response200
```

Get the evaluation of an order

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new cbdesk\Mirakl\Api\OrdersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

$associative_array = [
    'order_id' => 'order_id_example', // string
    'shop_id' => 56, // int | Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used.
    'locale' => 'locale_example', // string | &lt;ISO-639&gt;_&lt;ISO-3166&gt; (\"en_US\") or &lt;ISO-639&gt; (\"en\") locale for internationalized data translation. The APIs only accept locales that are equivalent to the languages activated in the back-office.
];

try {
    $result = $apiInstance->oR51($associate_array);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling OrdersApi->oR51: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Note: the input parameter is an associative array with the keys listed as the parameter names below.

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **order_id** | **string**|  | |
| **shop_id** | **int**| Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used. | [optional] |
| **locale** | **string**| &amp;lt;ISO-639&amp;gt;_&amp;lt;ISO-3166&amp;gt; (\&quot;en_US\&quot;) or &amp;lt;ISO-639&amp;gt; (\&quot;en\&quot;) locale for internationalized data translation. The APIs only accept locales that are equivalent to the languages activated in the back-office. | [optional] |

### Return type

[**\cbdesk\Mirakl\Model\OR51Response200**](../Model/OR51Response200.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `oR72()`

```php
oR72($order_ids, $shop_id): \cbdesk\Mirakl\Model\OR72Response200
```

Lists order's documents

Returns a list of all the documents available on the order

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new cbdesk\Mirakl\Api\OrdersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

$associative_array = [
    'order_ids' => 'order_ids_example', // string | the orders' identifiers, using comma as separator
    'shop_id' => 56, // int | Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used.
];

try {
    $result = $apiInstance->oR72($associate_array);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling OrdersApi->oR72: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Note: the input parameter is an associative array with the keys listed as the parameter names below.

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **order_ids** | **string**| the orders&#39; identifiers, using comma as separator | [optional] |
| **shop_id** | **int**| Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used. | [optional] |

### Return type

[**\cbdesk\Mirakl\Model\OR72Response200**](../Model/OR72Response200.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `oR73()`

```php
oR73($order_ids, $document_ids, $document_codes, $shop_id): \SplFileObject
```

Download one or multiple documents attached to one or multiple orders

<ul>   <li>If a list of document identifiers is specified only these documents are downloaded.       <ul>           <li>If more than one document id is specified, the documents will be wrapped in a ZIP archive</li>           <li>If only one document id is specified the document will not be zipped</li>       </ul>   </li>   <li>If a list of order identifiers is specified, all documents from those orders are downloaded.<br/>   Use a list of order document type codes to retrieve specific types from those orders.<br/>   In this case, the output of the API will always be a ZIP archive even if there is only one document to retrieve.   </li></ul>When documents are retrieved, they're wrapped into a ZIP archive except when only one document id is specified. The tree structure of this archive is as follow:<pre> documents-timestamp.zip | |__ order_id_x/ |   |__ foo.txt |   |__ bar.txt |   |__ baz.pdf | |__ order_id_y/ |   |__ image.png |   |__ image(1).png </pre>

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new cbdesk\Mirakl\Api\OrdersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

$associative_array = [
    'order_ids' => 'order_ids_example', // string | A list of identifiers of the orders (separated by a comma)
    'document_ids' => 'document_ids_example', // string | A list of document identifiers (separated by a comma)
    'document_codes' => 'document_codes_example', // string | A list of document type codes (separated by a comma)
    'shop_id' => 56, // int | Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used.
];

try {
    $result = $apiInstance->oR73($associate_array);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling OrdersApi->oR73: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Note: the input parameter is an associative array with the keys listed as the parameter names below.

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **order_ids** | **string**| A list of identifiers of the orders (separated by a comma) | [optional] |
| **document_ids** | **string**| A list of document identifiers (separated by a comma) | [optional] |
| **document_codes** | **string**| A list of document type codes (separated by a comma) | [optional] |
| **shop_id** | **int**| Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used. | [optional] |

### Return type

**\SplFileObject**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/octet-stream`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `oR75()`

```php
oR75($shop_id, $locale): \cbdesk\Mirakl\Model\OR75Response200
```

List all the order taxes available on the platform

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new cbdesk\Mirakl\Api\OrdersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

$associative_array = [
    'shop_id' => 56, // int | Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used.
    'locale' => 'locale_example', // string | &lt;ISO-639&gt;_&lt;ISO-3166&gt; (\"en_US\") or &lt;ISO-639&gt; (\"en\") locale for internationalized data translation. The APIs only accept locales that are equivalent to the languages activated in the back-office.
];

try {
    $result = $apiInstance->oR75($associate_array);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling OrdersApi->oR75: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Note: the input parameter is an associative array with the keys listed as the parameter names below.

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **shop_id** | **int**| Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used. | [optional] |
| **locale** | **string**| &amp;lt;ISO-639&amp;gt;_&amp;lt;ISO-3166&amp;gt; (\&quot;en_US\&quot;) or &amp;lt;ISO-639&amp;gt; (\&quot;en\&quot;) locale for internationalized data translation. The APIs only accept locales that are equivalent to the languages activated in the back-office. | [optional] |

### Return type

[**\cbdesk\Mirakl\Model\OR75Response200**](../Model/OR75Response200.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `oR76()`

```php
oR76($document_id, $shop_id)
```

Delete an order document

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new cbdesk\Mirakl\Api\OrdersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

$associative_array = [
    'document_id' => 56, // int | Identifier of the document to delete
    'shop_id' => 56, // int | Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used.
];

try {
    $apiInstance->oR76($associate_array);
} catch (Exception $e) {
    echo 'Exception when calling OrdersApi->oR76: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Note: the input parameter is an associative array with the keys listed as the parameter names below.

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **document_id** | **int**| Identifier of the document to delete | |
| **shop_id** | **int**| Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used. | [optional] |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
