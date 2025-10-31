# # P11Response200ProductsOffersDiscount

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**discount_price** | **float** | Discount price. Not to be read if discount with ranges is specified (i.e. discount with at least one range with quantity threshold greater than one). &lt;br/&gt;For Dropship specifically: the purchasing discount price. | [optional]
**end_date** | **\DateTime** | Discount end date | [optional]
**origin_price** | **float** | Origin price &lt;br/&gt;For Dropship specifically: the origin purchasing price | [optional]
**ranges** | [**\cbdesk\Mirakl\Model\P11Response200ProductsOffersDiscountRanges[]**](P11Response200ProductsOffersDiscountRanges.md) | Discount ranges | [optional]
**start_date** | **\DateTime** | Discount start date | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
