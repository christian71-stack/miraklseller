# # TL02Response200Data

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**accounting_document_creation_date** | **\DateTime** | The billing cycle&#39;s accounting document creation date | [optional]
**accounting_document_id** | **string** | The billing cycle&#39;s accounting document id. This field is only available for documents requests of the type: &lt;code&gt;SHOP_BILLING_CYCLE_PURCHASE_ORDER&lt;/code&gt;. | [optional]
**accounting_document_number** | **string** | The billing cycle&#39;s accounting document number | [optional]
**amount** | **int** | The amount. | [optional]
**amount_credited** | **int** | The amount credited. | [optional]
**amount_debited** | **int** | The amount debited. | [optional]
**balance** | **int** | The balance of the transaction. | [optional]
**currency_iso_code** | **string** | The currency of the shop (iso format) | [optional]
**date_created** | **\DateTime** | Creation date of the transaction line | [optional]
**entities** | [**\cbdesk\Mirakl\Model\TL02Response200DataEntities**](TL02Response200DataEntities.md) |  | [optional]
**id** | **string** | Identifier of the transaction | [optional]
**last_updated** | **\DateTime** | Date of last update of the transaction line | [optional]
**pay_out_psp_code** | **string** | Pay-out PSP code associated with the transaction. | [optional]
**payment_state** | **string** | The payment state of the transaction. | [optional]
**psp_balance** | **int** | The Pay-out balance of the transaction. | [optional]
**type** | **string** | Type of transaction (refund, transaction fee, etc ...) | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
