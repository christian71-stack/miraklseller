# # OR32Response200OrderLinesAdjustedCancelations

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount** | **float** | The offer part amount canceled | [optional]
**currency_iso_code** | **string** |  | [optional]
**eco_contributions** | [**\cbdesk\Mirakl\Model\OR32Response200OrderLinesAdjustedCancelationsEcoContributions[]**](OR32Response200OrderLinesAdjustedCancelationsEcoContributions.md) | List of eco-contribution amounts and corresponding producer identifiers, if applicable&lt;br/&gt; Only available if the operator activates the circular economy information collection. | [optional]
**quantity** | **int** | The quantity of goods canceled | [optional]
**reason_code** | **string** | Cancellation&#39;s reason code | [optional]
**shipping_amount** | **float** | The shipping charges part amount canceled | [optional]
**shipping_taxes** | [**\cbdesk\Mirakl\Model\OR32Response200OrderLinesAdjustedCancelationsShippingTaxes[]**](OR32Response200OrderLinesAdjustedCancelationsShippingTaxes.md) | The taxes canceled on the shipping price | [optional]
**taxes** | [**\cbdesk\Mirakl\Model\OR32Response200OrderLinesAdjustedCancelationsTaxes[]**](OR32Response200OrderLinesAdjustedCancelationsTaxes.md) | The taxes canceled on the product price | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
