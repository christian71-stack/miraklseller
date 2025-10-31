# # OR13Request

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_codes** | **string[]** | A list of channel codes | [optional]
**end_date** | **\DateTime** | End order creation date for filtering. Must be used with &lt;code&gt;start_date&lt;/code&gt;. | [optional]
**end_update_date** | **\DateTime** | End order update date for filtering. Must be used with &lt;code&gt;start_update_date&lt;/code&gt;. | [optional]
**fulfillment_center_codes** | **string** | Code of the fulfillment center | [optional]
**items_per_chunk** | **int** | Maximum number of items included in the generated files | [optional] [default to 1000000]
**megabytes_per_chunk** | **int** | Maximum mega bytes weight for generated files | [optional] [default to 512]
**only_null_channel** | **bool** | Return only orders without channel. If &lt;code&gt;true&lt;/code&gt;, ignore the &lt;code&gt;channel_codes&lt;/code&gt; | [optional] [default to false]
**order_state_codes** | **string[]** | A list of order state&#39;s codes | [optional]
**order_tax_mode** | **string** | Please note: If the taxes are not specified, the prices with mode TAX_EXCLUDED and with mode TAX_INCLUDED will return the same amounts.&lt;br&gt;Possible values:&lt;ul&gt;&lt;li&gt;&lt;code&gt;TAX_EXCLUDED&lt;/code&gt;: the price fields (price, unit price, shipping price, cancellation amount, refund amount and order total prices) do not include taxes.&lt;/li&gt;&lt;li&gt;&lt;code&gt;TAX_INCLUDED&lt;/code&gt;: the price fields include the tax amount. &lt;/li&gt;&lt;/ul&gt;&lt;li&gt;If this query parameter is not specified, the default order tax mode of the platform is used.&lt;/li&gt; | [optional]
**start_date** | **\DateTime** | Start order creation date for filtering. Must be used with &lt;code&gt;end_date&lt;/code&gt;. | [optional]
**start_update_date** | **\DateTime** | Start order update date for filtering. Mirakl will subtract a time delta to ensure no orders are missed due to network and/or software latency. Must be used with &lt;code&gt;end_update_date&lt;/code&gt;. | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
