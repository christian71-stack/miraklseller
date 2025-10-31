# # OF24RequestOffersDiscount

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**end_date** | **string** | Discount end date. May be required when a discount price is set, check platform configuration. Offer update: if not provided, existing data will be deleted. | [optional]
**price** | **float** | Discount price. Not to be used when ranges are specified. Offer update: if not provided, existing data will be deleted. For Dropship specifically: the discount purchasing price of the offer, also referred to as discount cost or discount wholesale price. | [optional]
**ranges** | [**\cbdesk\Mirakl\Model\OF24RequestOffersDiscountRanges[]**](OF24RequestOffersDiscountRanges.md) | Discount ranges. Offer update: if not provided, existing data will be deleted. | [optional]
**start_date** | **string** | Discount start date. May be required when a discount price is set, check platform configuration. Offer update: if not provided, existing data will be deleted. | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
