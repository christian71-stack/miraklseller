# # IV01Response200InvoicesDetails

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount_excl_taxes** | **float** | Amount excluding taxes | [optional]
**description** | **string** | Description | [optional]
**operation_date** | **\DateTime** | Operation date for &lt;code&gt;MANUAL_INVOICE&lt;/code&gt; or &lt;code&gt;MANUAL_CREDIT&lt;/code&gt; type | [optional]
**order_id** | **string** | Associated order id. Only for &lt;code&gt;MANUAL_INVOICE&lt;/code&gt; or &lt;code&gt;MANUAL_CREDIT&lt;/code&gt; type | [optional]
**quantity** | **int** | Quantity | [optional]
**taxes** | [**\cbdesk\Mirakl\Model\IV01Response200InvoicesDetailsTaxes[]**](IV01Response200InvoicesDetailsTaxes.md) | Taxes | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
