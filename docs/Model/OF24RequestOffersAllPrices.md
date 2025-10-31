# # OF24RequestOffersAllPrices

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_code** | **string** | The channel code the prices will be linked to. To set the default prices, set it to null. | [optional]
**discount_end_date** | **string** | The end date of the discount. May be required when a discount price is set, check platform configuration. If no discount is desired, set it to null. | [optional]
**discount_start_date** | **string** | The start date of the discount. May be required when a discount price is set, check platform configuration. If no discount is desired, set it to null. | [optional]
**unit_discount_price** | **float** | The default unit discount price, i.e. the unit price when the discount applied. | [optional]
**unit_origin_price** | **float** | The default unit original price, i.e. the unit price without taking discounts nor volume prices into account. | [optional]
**volume_prices** | [**\cbdesk\Mirakl\Model\OF24RequestOffersAllPricesVolumePrices[]**](OF24RequestOffersAllPricesVolumePrices.md) | The volume prices applicable for the offer. | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
