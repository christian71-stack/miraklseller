# # P51Response200ProductImportTrackings

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**conversion_options** | [**\cbdesk\Mirakl\Model\P51Response200ProductImportTrackingsConversionOptions**](P51Response200ProductImportTrackingsConversionOptions.md) |  | [optional]
**conversion_type** | **string** | Type of conversion applied on products | [optional]
**date_created** | **\DateTime** | Import creation date | [optional]
**has_error_report** | **bool** | Returns true if error report is available. Value is filled when the import is completed | [optional]
**has_new_product_report** | **bool** | Returns true if new product report is available. Value is filled when the import is completed | [optional]
**has_transformation_error_report** | **bool** | Returns true if transformation error report is available. Value is filled when the import is completed | [optional]
**has_transformed_file** | **bool** | Returns true if transformed file is available. Value is filled when the import is completed | [optional]
**import_id** | **int** | Import identifier | [optional]
**import_status** | **string** | Import status | [optional]
**integration_details** | [**\cbdesk\Mirakl\Model\P51Response200ProductImportTrackingsIntegrationDetails**](P51Response200ProductImportTrackingsIntegrationDetails.md) |  | [optional]
**reason_status** | **string** | A message explaining the reason of the import status, if relevant | [optional]
**shop_id** | **int** | Shop identifier | [optional]
**transform_lines_in_error** | **int** | Total count of transformed lines in error | [optional]
**transform_lines_in_success** | **int** | Total count of transformed lines in success | [optional]
**transform_lines_read** | **int** | Total count of transformed lines read | [optional]
**transform_lines_with_warning** | **int** | Total count of transformed lines with warning | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
