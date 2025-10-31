# # OR11Response200OrdersPromotionsAppliedPromotionsConfiguration

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount_off** | **float** | The amount off of the promotion. &lt;br/&gt;Only applicable when promotion is of type &lt;code&gt;AMOUNT_OFF&lt;/code&gt;, null otherwise. | [optional]
**free_items_quantity** | **int** | The free item target quantity of the promotion. &lt;br/&gt;Only applicable when promotion is of type &lt;code&gt;FREE_ITEMS&lt;/code&gt;, null otherwise. | [optional]
**internal_description** | **string** | Promotion&#39;s Internal description, set by the shop at creation | [optional]
**percentage_off** | **float** | The percentage off of the promotion. &lt;br/&gt;Only applicable when promotion is of type &lt;code&gt;PERCENTAGE_OFF&lt;/code&gt;, null otherwise. | [optional]
**reduced_unit_price** | **float** | The new offer’s unit price triggered by the promotion. &lt;br/&gt;Only applicable when promotion is of type &lt;code&gt;REDUCED_UNIT_PRICE&lt;/code&gt;, null otherwise. | [optional]
**type** | **string** | Promotion&#39;s type, whether it is applied to this item (&lt;code&gt;ITEM&lt;/code&gt;), or every items in the basket for this shop (&lt;code&gt;BASKET&lt;/code&gt;) | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
