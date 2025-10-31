# # A02Request

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**address** | [**\cbdesk\Mirakl\Model\A02RequestAddress**](A02RequestAddress.md) |  | [optional]
**channels** | **string[]** | List of the channel codes associated to the shop. If new channel is associated without providing values for the required shop_additional_fields, default values will be set. | [optional]
**closed_from** | **\DateTime** | Date: if defined, this shop will be closed on this date. Nullable. | [optional]
**closed_to** | **\DateTime** | Date: if defined, this shop will be reopened on this date. Nullable. | [optional]
**description** | **string** | Description of the shop. Nullable. | [optional]
**email** | **string** | Email of the shop. Cannot be null. | [optional]
**fax** | **string** | Fax of the shop. Nullable. | [optional]
**is_professional** | **bool** | Whether or not the shop is professional. Cannot be null. | [optional]
**payment_info** | [**\cbdesk\Mirakl\Model\A02RequestPaymentInfo**](A02RequestPaymentInfo.md) |  | [optional]
**pro_details** | [**\cbdesk\Mirakl\Model\A02RequestProDetails**](A02RequestProDetails.md) |  | [optional]
**producer_identifiers** | [**\cbdesk\Mirakl\Model\A02RequestProducerIdentifiers[]**](A02RequestProducerIdentifiers.md) | List of shop’s producer identifiers per Extended Producer Responsibility (EPR) categories. Only available if the operator setting &lt;em&gt;Activate data collection related to circular economy regulations&lt;/em&gt; is enabled. | [optional]
**recycling_policy** | **string** | Recycling policy - only available if the operator setting &lt;em&gt;Activate data collection related to circular economy regulations&lt;/em&gt; has been enabled. | [optional]
**return_policy** | **string** | Return policy of the shop. Nullable. | [optional]
**shipping_country** | **string** | Shipping country of the shop. Nullable. | [optional]
**shop_additional_fields** | [**\cbdesk\Mirakl\Model\A02RequestShopAdditionalFields[]**](A02RequestShopAdditionalFields.md) | Additional fields of the shop. Note that if the &#39;value&#39; field in the child structure is absent, the corresponding additional field value will be removed for this shop. Nullable. | [optional]
**shop_name** | **string** | The name of the shop. Cannot be null. | [optional]
**web_site** | **string** | Website of the shop. Nullable. | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
