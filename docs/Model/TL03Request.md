# # TL03Request

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**accounting_document_id** | **string** | Accounting document id for filtering. This parameter only filter documents requests of the type: &lt;code&gt;SHOP_BILLING_CYCLE_PURCHASE_ORDER&lt;/code&gt;. | [optional]
**accounting_document_number** | **string** | Accounting document number for filtering. | [optional]
**date_created_from** | **\DateTime** | Creation date for filtering | [optional]
**date_created_to** | **\DateTime** | Creation date for filtering | [optional]
**items_per_chunk** | **int** | The maximum number of items per chunk. | [optional]
**last_updated_from** | **\DateTime** | Last updated date for filtering | [optional]
**megabytes_per_chunk** | **int** | The maximum size in megabytes of a chunk. | [optional]
**order_id** | **string[]** | Order id for filtering. This parameter can be supplied multiple times. | [optional]
**order_line_id** | **string[]** | Order line id for filtering. This parameter can be supplied multiple times. | [optional]
**order_reference_for_customer** | **string[]** | A comma-separated list of order references for customer. | [optional]
**order_reference_for_seller** | **string[]** | A comma-separated list of order references for seller. | [optional]
**pay_out_psp_codes** | **string[]** | A comma-separated list of pay-out PSP codes for filtering. This parameter requires the Hybrid pay-out PSP feature to be enabled. | [optional]
**payment_state** | **string[]** | Payment state for filtering. This parameter can be supplied multiple times. | [optional]
**payment_voucher_number** | **string** | Payment voucher for filtering | [optional]
**shop_domain** | **string[]** | A shop domain for filtering. This parameter can be supplied multiple times. | [optional]
**shop_id** | **int** | Shop identifier | [optional]
**shop_model** | **string[]** | Shop model for filtering. This parameter can be supplied multiple times. | [optional]
**transaction_date_from** | **\DateTime** | Transaction date for filtering | [optional]
**transaction_date_to** | **\DateTime** | Transaction date for filtering | [optional]
**transaction_type** | **string[]** | Transaction type for filtering. This parameter can be supplied multiple times. | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
