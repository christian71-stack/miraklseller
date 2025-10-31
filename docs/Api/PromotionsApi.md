# cbdesk\Mirakl\PromotionsApi



All URIs are relative to https://your-instance.mirakl.net, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**pR01()**](PromotionsApi.md#pR01) | **GET** /api/promotions | List promotions |


## `pR01()`

```php
pR01($ids, $types, $states, $ending_after, $starting_before, $date_created_from, $date_created_to, $last_request_date, $locale, $trigger_offer_ids, $reward_offer_ids, $channel_codes, $shop_id, $max, $offset, $sort, $order): \cbdesk\Mirakl\Model\PR01Response200
```

List promotions

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new cbdesk\Mirakl\Api\PromotionsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

$associative_array = [
    'ids' => 'ids_example', // string | A comma separated list of identifiers for a promotion
    'types' => 'types_example', // string | A comma separated list of types for a promotion [AMOUNT_OFF|FREE_ITEMS|PERCENTAGE_OFF|REDUCED_UNIT_PRICE]
    'states' => 'ACTIVE', // string | A comma separated list of states for a promotion [PENDING|ACTIVE|EXPIRED|PENDING_APPROVAL|REJECTED|ALL]
    'ending_after' => new \DateTime('2013-10-20T19:20:30+01:00'), // \DateTime | Returns promotions which ended or will end after this date
    'starting_before' => new \DateTime('2013-10-20T19:20:30+01:00'), // \DateTime | Returns promotions which started or will start before this date
    'date_created_from' => new \DateTime('2013-10-20T19:20:30+01:00'), // \DateTime | Filter promotion creation date lower limit
    'date_created_to' => new \DateTime('2013-10-20T19:20:30+01:00'), // \DateTime | Filter promotion creation date upper limit
    'last_request_date' => new \DateTime('2013-10-20T19:20:30+01:00'), // \DateTime | Last request date and time. We recommend using the differential mode along with the <code>states</code> parameter.
    'locale' => 'locale_example', // string | The locale to filter the medias and the public descriptions with. If not specified, medias and public descriptions of all locales are returned.If specified, only the media and the public description matching the locale will be returned, or, if not exist, the one matching the platform default locale.
    'trigger_offer_ids' => 'trigger_offer_ids_example', // string | Promotion-triggering offer ids, separated by commas
    'reward_offer_ids' => 'reward_offer_ids_example', // string | Promotion reward offer ids, separated by commas
    'channel_codes' => 'channel_codes_example', // string | Channel codes on which promotions apply, separated by commas
    'shop_id' => 56, // int | Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used.
    'max' => 56, // int | Maximum number of items returned per page
    'offset' => 56, // int | Index of the first item (among all the results) in the returned page
    'sort' => 'sort_example', // string | How the results should be sorted
    'order' => 'order_example', // string | Sort direction
];

try {
    $result = $apiInstance->pR01($associate_array);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PromotionsApi->pR01: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Note: the input parameter is an associative array with the keys listed as the parameter names below.

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **ids** | **string**| A comma separated list of identifiers for a promotion | [optional] |
| **types** | **string**| A comma separated list of types for a promotion [AMOUNT_OFF|FREE_ITEMS|PERCENTAGE_OFF|REDUCED_UNIT_PRICE] | [optional] |
| **states** | **string**| A comma separated list of states for a promotion [PENDING|ACTIVE|EXPIRED|PENDING_APPROVAL|REJECTED|ALL] | [optional] [default to &#39;ACTIVE&#39;] |
| **ending_after** | **\DateTime**| Returns promotions which ended or will end after this date | [optional] |
| **starting_before** | **\DateTime**| Returns promotions which started or will start before this date | [optional] |
| **date_created_from** | **\DateTime**| Filter promotion creation date lower limit | [optional] |
| **date_created_to** | **\DateTime**| Filter promotion creation date upper limit | [optional] |
| **last_request_date** | **\DateTime**| Last request date and time. We recommend using the differential mode along with the &lt;code&gt;states&lt;/code&gt; parameter. | [optional] |
| **locale** | **string**| The locale to filter the medias and the public descriptions with. If not specified, medias and public descriptions of all locales are returned.If specified, only the media and the public description matching the locale will be returned, or, if not exist, the one matching the platform default locale. | [optional] |
| **trigger_offer_ids** | **string**| Promotion-triggering offer ids, separated by commas | [optional] |
| **reward_offer_ids** | **string**| Promotion reward offer ids, separated by commas | [optional] |
| **channel_codes** | **string**| Channel codes on which promotions apply, separated by commas | [optional] |
| **shop_id** | **int**| Use this parameter when your user has access to several shops. If not specified, the shop_id from your default shop will be used. | [optional] |
| **max** | **int**| Maximum number of items returned per page | [optional] |
| **offset** | **int**| Index of the first item (among all the results) in the returned page | [optional] |
| **sort** | **string**| How the results should be sorted | [optional] |
| **order** | **string**| Sort direction | [optional] |

### Return type

[**\cbdesk\Mirakl\Model\PR01Response200**](../Model/PR01Response200.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
