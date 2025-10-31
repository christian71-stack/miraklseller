# # IV01Response200Invoices

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**currency_iso_code** | **string** | The currency of the shop | [optional]
**date_created** | **\DateTime** | Accounting document creation date | [optional]
**details** | [**\cbdesk\Mirakl\Model\IV01Response200InvoicesDetails[]**](IV01Response200InvoicesDetails.md) | Accounting details | [optional]
**due_date** | **\DateTime** | Due date for the payment of the accounting document | [optional]
**id** | **string** | Accounting document identifier (use it for draft document) | [optional]
**invoice_id** | **int** | Accounting document identifier (present if the accounting document is issued) | [optional]
**issue_date** | **\DateTime** | Issue date of an accounting document | [optional]
**issuing_user** | [**\cbdesk\Mirakl\Model\IV01Response200InvoicesIssuingUser**](IV01Response200InvoicesIssuingUser.md) |  | [optional]
**pay_out_psp_code** | **string** | PSP code for Pay-out | [optional]
**payment** | [**\cbdesk\Mirakl\Model\IV01Response200InvoicesPayment**](IV01Response200InvoicesPayment.md) |  | [optional]
**shop_address** | [**\cbdesk\Mirakl\Model\IV01Response200InvoicesShopAddress**](IV01Response200InvoicesShopAddress.md) |  | [optional]
**shop_corporate_name** | **string** | Shop corporate name if it is a professional shop | [optional]
**shop_id** | **int** | Shop id | [optional]
**shop_model** | **string** | Shop model | [optional]
**shop_name** | **string** | Shop name | [optional]
**shop_operator_internal_id** | **string** | Operator internal id for the shop | [optional]
**shop_tax_number** | **string** | Shop tax number if it is a professional shop | [optional]
**state** | **string** | Accounting document state | [optional]
**total_amount_excl_taxes** | **float** | Total amount charged to the shop (excluding taxes) | [optional]
**total_amount_incl_taxes** | **float** | Total amount charged to the shop (including taxes) | [optional]
**total_taxes** | [**\cbdesk\Mirakl\Model\IV01Response200InvoicesTotalTaxes[]**](IV01Response200InvoicesTotalTaxes.md) | Total taxes | [optional]
**type** | **string** | Accounting document type | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
