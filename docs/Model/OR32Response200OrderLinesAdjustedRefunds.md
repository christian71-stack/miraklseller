# # OR32Response200OrderLinesAdjustedRefunds

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount** | **float** | The offer part amount refunded. | [optional]
**currency_iso_code** | **string** |  | [optional]
**eco_contributions** | [**\cbdesk\Mirakl\Model\OR32Response200OrderLinesAdjustedRefundsEcoContributions[]**](OR32Response200OrderLinesAdjustedRefundsEcoContributions.md) | List of eco-contribution amounts and corresponding producer identifiers, if applicable&lt;br/&gt; Only available if the operator activates the circular economy information collection. | [optional]
**quantity** | **int** | The quantity of products refunded. This quantity is informative only. | [optional]
**reason_code** | **string** | Refund&#39;s reason code | [optional]
**shipping_amount** | **float** | The shipping charges part amount refunded | [optional]
**shipping_taxes** | [**\cbdesk\Mirakl\Model\OR32Response200OrderLinesAdjustedRefundsShippingTaxes[]**](OR32Response200OrderLinesAdjustedRefundsShippingTaxes.md) | The taxes refunded on the shipping price | [optional]
**taxes** | [**\cbdesk\Mirakl\Model\OR32Response200OrderLinesAdjustedRefundsTaxes[]**](OR32Response200OrderLinesAdjustedRefundsTaxes.md) | The taxes refunded on the product price | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
