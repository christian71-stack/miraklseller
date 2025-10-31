# # DR12Response200Data

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**delivery_bill_information** | [**\cbdesk\Mirakl\Model\DR12Response200DataDeliveryBillInformation[]**](DR12Response200DataDeliveryBillInformation.md) | Delivery bill information | [optional]
**eco_contributions** | [**\cbdesk\Mirakl\Model\DR12Response200DataEcoContributions[]**](DR12Response200DataEcoContributions.md) | List of eco-contribution amounts and corresponding producer identifiers, if applicable&lt;br/&gt; Only available if the operator activates the circular economy information collection. | [optional]
**entity_id** | **string** | The entity id the document line relates to | [optional]
**entity_type** | **string** | The entity type the document line relates to | [optional]
**fees_excluding_taxes** | [**\cbdesk\Mirakl\Model\DR12Response200DataFeesExcludingTaxes[]**](DR12Response200DataFeesExcludingTaxes.md) | List of fees applied on the order line | [optional]
**order** | [**\cbdesk\Mirakl\Model\DR12Response200DataOrder**](DR12Response200DataOrder.md) |  | [optional]
**order_line** | [**\cbdesk\Mirakl\Model\DR12Response200DataOrderLine**](DR12Response200DataOrderLine.md) |  | [optional]
**origin_unit_price_excluding_taxes** | **float** | The original unit price excluding tax of the offer associated with the order line | [optional]
**origin_unit_price_including_taxes** | **float** | The original unit price including tax of the offer associated with the order line | [optional]
**payment_state** | **string** | Document request line payment status | [optional]
**price_excluding_taxes** | **float** | The price excluding taxes after promotions | [optional]
**product** | [**\cbdesk\Mirakl\Model\DR12Response200DataProduct**](DR12Response200DataProduct.md) |  | [optional]
**quantity** | **int** | The quantity of the document line | [optional]
**shipping_from** | [**\cbdesk\Mirakl\Model\DR12Response200DataShippingFrom**](DR12Response200DataShippingFrom.md) |  | [optional]
**shipping_price_excluding_taxes** | **float** | The shipping price excluding taxes | [optional]
**shipping_taxes** | [**\cbdesk\Mirakl\Model\DR12Response200DataShippingTaxes[]**](DR12Response200DataShippingTaxes.md) | The shipping taxes | [optional]
**shipping_to** | [**\cbdesk\Mirakl\Model\DR12Response200DataShippingTo**](DR12Response200DataShippingTo.md) |  | [optional]
**shop** | [**\cbdesk\Mirakl\Model\DR12Response200DataShop**](DR12Response200DataShop.md) |  | [optional]
**tax_legal_notice** | **string** | The legal notice applying to the offer’s tax calculation | [optional]
**taxes** | [**\cbdesk\Mirakl\Model\DR12Response200DataTaxes[]**](DR12Response200DataTaxes.md) | The taxes | [optional]
**total_price_including_taxes** | **float** | The total price | [optional]
**unit_price_excluding_taxes** | **float** | The unit price excluding taxes after promotions | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
