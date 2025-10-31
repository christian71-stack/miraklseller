# # ST01Response201ShipmentSuccessTracking

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**carrier_code** | **string** | The code of a carrier. This information is mandatory for a registered carrier. | [optional]
**carrier_expected_delivery_date** | [**\cbdesk\Mirakl\Model\ST01Response201ShipmentSuccessTrackingCarrierExpectedDeliveryDate**](ST01Response201ShipmentSuccessTrackingCarrierExpectedDeliveryDate.md) |  | [optional]
**carrier_name** | **string** | The name of a carrier. This information is mandatory for an unregistered carrier. | [optional]
**carrier_standard_code** | **string** | The standard code of a carrier based on mirakl carrier referential | [optional]
**last_known_location** | [**\cbdesk\Mirakl\Model\ST01Response201ShipmentSuccessTrackingLastKnownLocation**](ST01Response201ShipmentSuccessTrackingLastKnownLocation.md) |  | [optional]
**milestones** | [**\cbdesk\Mirakl\Model\ST01Response201ShipmentSuccessTrackingMilestones[]**](ST01Response201ShipmentSuccessTrackingMilestones.md) | Retrieves the main stages of the delivery of a shipment coming from carrier&#39;s systems | [optional]
**tracking_number** | **string** | The carrier tracking number. This information is mandatory for a registered carrier with a URL requiring a tracking number. | [optional]
**tracking_url** | **string** | The tracking url of a carrier. This information is unused for registered carriers (because computed automatically). This information is optional for unregistered carriers. | [optional]
**validity_status** | **string** | Retrieves if mirakl is able to get tracking information (if not, then unverified) and if we manage to get tracking information and if we do get tracking information on this tracking, then it moves to verified, if we don&#39;t it remains in unverified | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
