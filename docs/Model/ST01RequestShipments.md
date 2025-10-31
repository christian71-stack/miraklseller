# # ST01RequestShipments

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**invoice_reference** | **string** | Shipment&#39;s invoice reference | [optional]
**order_id** | **string** | Order identifier | [optional]
**shipment_additional_information** | [**\cbdesk\Mirakl\Model\ST01RequestShipmentsShipmentAdditionalInformation[]**](ST01RequestShipmentsShipmentAdditionalInformation.md) | Shipment&#39;s additional information | [optional]
**shipment_lines** | [**\cbdesk\Mirakl\Model\ST01RequestShipmentsShipmentLines[]**](ST01RequestShipmentsShipmentLines.md) | Shipment lines | [optional]
**shipped** | **bool** | If true, the shipment is shipped after its creation | [optional] [default to false]
**shipping_from** | [**\cbdesk\Mirakl\Model\ST01RequestShipmentsShippingFrom**](ST01RequestShipmentsShippingFrom.md) |  | [optional]
**tracking** | [**\cbdesk\Mirakl\Model\ST01RequestShipmentsTracking**](ST01RequestShipmentsTracking.md) |  | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
