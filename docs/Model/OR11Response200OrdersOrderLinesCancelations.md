# # OR11Response200OrdersOrderLinesCancelations

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount** | **float** | Cancellation&#39;s amount | [optional]
**amount_breakdown** | [**\cbdesk\Mirakl\Model\OR11Response200OrdersOrderLinesCancelationsAmountBreakdown**](OR11Response200OrdersOrderLinesCancelationsAmountBreakdown.md) |  | [optional]
**commission_amount** | **float** | Cancellation&#39;s commission amount | [optional]
**commission_taxes** | [**\cbdesk\Mirakl\Model\OR11Response200OrdersOrderLinesCancelationsCommissionTaxes[]**](OR11Response200OrdersOrderLinesCancelationsCommissionTaxes.md) | Cancellation&#39;s commission taxes | [optional]
**commission_total_amount** | **float** | The total commission amount of the cancellation (commission amount + commission taxes) | [optional]
**created_date** | **\DateTime** | Cancellation&#39;s creation date | [optional]
**eco_contributions** | [**\cbdesk\Mirakl\Model\OR11Response200OrdersOrderLinesCancelationsEcoContributions[]**](OR11Response200OrdersOrderLinesCancelationsEcoContributions.md) | List of eco-contribution amounts and corresponding producer identifiers, if applicable&lt;br/&gt; Only available if the operator activates the circular economy information collection. | [optional]
**fees** | [**\cbdesk\Mirakl\Model\OR11Response200OrdersOrderLinesCancelationsFees[]**](OR11Response200OrdersOrderLinesCancelationsFees.md) | List of fees canceled on the order line | [optional]
**id** | **string** | Cancellation&#39;s id | [optional]
**purchase_information** | [**\cbdesk\Mirakl\Model\OR11Response200OrdersOrderLinesCancelationsPurchaseInformation**](OR11Response200OrdersOrderLinesCancelationsPurchaseInformation.md) |  | [optional]
**quantity** | **int** | The quantity of products canceled (This quantity is informative only) | [optional]
**reason_code** | **string** | Cancellation reason&#39;s code | [optional]
**shipping_amount** | **float** | Cancellation&#39;s shipping amount | [optional]
**shipping_amount_breakdown** | [**\cbdesk\Mirakl\Model\OR11Response200OrdersOrderLinesCancelationsShippingAmountBreakdown**](OR11Response200OrdersOrderLinesCancelationsShippingAmountBreakdown.md) |  | [optional]
**shipping_taxes** | [**\cbdesk\Mirakl\Model\OR11Response200OrdersOrderLinesCancelationsShippingTaxes[]**](OR11Response200OrdersOrderLinesCancelationsShippingTaxes.md) | The taxes on the shipping price | [optional]
**taxes** | [**\cbdesk\Mirakl\Model\OR11Response200OrdersOrderLinesCancelationsTaxes[]**](OR11Response200OrdersOrderLinesCancelationsTaxes.md) | The taxes on the price | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
