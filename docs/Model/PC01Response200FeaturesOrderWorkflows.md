# # PC01Response200FeaturesOrderWorkflows

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**no_customer_payment_confirmation** | **bool** | Allows seller payments to be completely separated from customer debits | [optional]
**order_acceptance** | **string** | Indicate if shop accounts must accept new orders and take responsibility for the transaction. NOT_AUTOMATIC: All shop accounts must accept their orders manually. AUTOMATIC: Orders are automatically accepted. BOTH: AUTOMATIC or NOT_AUTOMATIC mode depending on the store account | [optional]
**pause_debit_workflow** | **bool** | Pause the order debit workflow when taxes must be recalculated | [optional]
**pay_on_due_date** | **bool** | Allows professionals to pay their orders after the receipt of the items or an explicit invoice | [optional]
**pay_on_shipment** | **bool** | Allows operators to debit orders before they have been fully shipped | [optional]
**sellers_edit_shipping_origin** | **bool** | Allow shop accounts to edit shipping origin to ensures accurate tax calculations with shipping origin data | [optional]
**shipping_and_billing_details_before_acceptance** | **bool** | Indicate if shipping and billing details are displayed before order acceptance | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
