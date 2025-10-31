# # ST01RequestShipmentsTracking

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**carrier_code** | **string** | The code of a carrier. This information is mandatory for a registered carrier. | [optional]
**carrier_name** | **string** | The name of a carrier. This information is mandatory for an unregistered carrier. | [optional]
**carrier_standard_code** | **string** | The standard code of a carrier based on mirakl carrier referential | [optional]
**tracking_number** | **string** | The carrier tracking number. This information is mandatory for a registered carrier with a URL requiring a tracking number. | [optional]
**tracking_url** | **string** | The tracking url of a carrier. This information is unused for registered carriers (because computed automatically). This information is optional for unregistered carriers. | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
