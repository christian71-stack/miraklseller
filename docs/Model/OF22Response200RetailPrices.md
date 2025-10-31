# # OF22Response200RetailPrices

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**discount_end_date** | **\DateTime** | End date of the discount, or null if no discount exists or if the discount does not have an end date. | [optional]
**discount_start_date** | **\DateTime** | Start date of the discount, or null if no discount exists or if the discount does not have a start date. | [optional]
**price** | **float** | Retail price of the offer, also referred to as selling price. &lt;br/&gt; If a discount is defined and is currently active (within the validity interval), it represents the unit_discount_price. &lt;br/&gt; In other cases, it represents the unit_origin_price. | [optional]
**unit_discount_price** | **float** | Discount retail price for a quantity of one, i.e. the discount retail price for a quantity of one. &lt;br/&gt; Set to null if no discount is defined or if no discount retail price for a quantity of one is defined or if the discount is not currently active (within the validity interval). | [optional]
**unit_origin_price** | **float** | Original retail price for a quantity of one, i.e. the retail price for a quantity of one regardless of the discounts. | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
