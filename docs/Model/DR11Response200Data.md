# # DR11Response200Data

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**currency_iso_code** | **string** | The currency of the document request | [optional]
**date_created** | **\DateTime** | The document request creation date | [optional]
**document_details** | [**\cbdesk\Mirakl\Model\DR11Response200DataDocumentDetails[]**](DR11Response200DataDocumentDetails.md) | The document details | [optional]
**document_number** | **string** | The accounting document number | [optional]
**document_upload_date** | **\DateTime** | The last upload date of the accounting document | [optional]
**due_date** | **\DateTime** | The document due date | [optional]
**entities** | [**\cbdesk\Mirakl\Model\DR11Response200DataEntities**](DR11Response200DataEntities.md) |  | [optional]
**entity_date_created** | **\DateTime** | The entity creation date, not applicable for entity_type&#x3D;SHOP_BILLING_CYCLE_PURCHASE_ORDER | [optional]
**entity_id** | **string** | The entity id the document request relates to | [optional]
**entity_type** | **string** | The entity type the document request relates to | [optional]
**id** | **string** | The document request unique identifier | [optional]
**initial_documents** | [**\cbdesk\Mirakl\Model\DR11Response200DataInitialDocuments[]**](DR11Response200DataInitialDocuments.md) | In the case of &lt;code&gt;CREDIT_NOTE&lt;/code&gt; or reissued &lt;code&gt;INVOICE&lt;/code&gt;, information about the initial accounting documents | [optional]
**initial_payment_state** | **string** | The document request payment state at the time when the document request was created | [optional]
**issue_date** | **\DateTime** | The document issue date | [optional]
**issuer** | [**\cbdesk\Mirakl\Model\DR11Response200DataIssuer**](DR11Response200DataIssuer.md) |  | [optional]
**last_updated** | **\DateTime** | The document request last update date | [optional]
**payment** | [**\cbdesk\Mirakl\Model\DR11Response200DataPayment**](DR11Response200DataPayment.md) |  | [optional]
**payment_destination** | [**\cbdesk\Mirakl\Model\DR11Response200DataPaymentDestination**](DR11Response200DataPaymentDestination.md) |  | [optional]
**payment_terms** | [**\cbdesk\Mirakl\Model\DR11Response200DataPaymentTerms**](DR11Response200DataPaymentTerms.md) |  | [optional]
**recipient** | [**\cbdesk\Mirakl\Model\DR11Response200DataRecipient**](DR11Response200DataRecipient.md) |  | [optional]
**state** | **string** | The document request state | [optional]
**taxes** | [**\cbdesk\Mirakl\Model\DR11Response200DataTaxes[]**](DR11Response200DataTaxes.md) | Total amount of taxes aggregated per tax code and rate | [optional]
**total_amount_excluding_taxes** | **float** | The total document amount (excluding taxes) | [optional]
**total_amount_including_taxes** | **float** | The total document amount (including taxes) | [optional]
**total_tax_amount** | **float** | The total taxes amount of the document | [optional]
**type** | **string** | The accounting document type | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
