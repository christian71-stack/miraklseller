# # PM11Response200Attributes

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channels** | [**\cbdesk\Mirakl\Model\PM11Response200AttributesChannels[]**](PM11Response200AttributesChannels.md) | Channels | [optional]
**code** | **string** | Attribute code | [optional]
**default_value** | **string** | Default value for value list type attributes | [optional]
**description** | **string** | Attribute description | [optional]
**description_translations** | [**\cbdesk\Mirakl\Model\PM11Response200AttributesDescriptionTranslations[]**](PM11Response200AttributesDescriptionTranslations.md) | Translations of the attribute description | [optional]
**example** | **string** | Attribute example to help sellers when they fill the product creation form | [optional]
**hierarchy_code** | **string** | The code of the hierarchy (category) this attribute belongs to. If this field is empty, the attribute is shared among all hierarchies. | [optional]
**label** | **string** | Attribute label | [optional]
**label_translations** | [**\cbdesk\Mirakl\Model\PM11Response200AttributesLabelTranslations[]**](PM11Response200AttributesLabelTranslations.md) | Translations of the attribute label | [optional]
**locale** | **string** | Attribute localization.&lt;br/&gt; The language format can either be:&lt;br/&gt; &lt;ul&gt;    &lt;li&gt;ISO-639 (E.g. \&quot;en\&quot;)&lt;/li&gt;    &lt;li&gt;ISO-639_ISO-3166 (E.g. \&quot;en_US\&quot;)&lt;/li&gt; &lt;/ul&gt; | [optional]
**required** | **bool** | Whether or not the attribute is required | [optional]
**requirement_level** | **string** | Requirement level of the attribute | [optional]
**roles** | [**\cbdesk\Mirakl\Model\PM11Response200AttributesRoles[]**](PM11Response200AttributesRoles.md) | Attribute roles | [optional]
**transformations** | **string** | Transformations applied to the attribute (a list of transformations separated by commas) | [optional]
**type** | **string** | Attribute type | [optional]
**type_parameter** | **string** | Type parameter | [optional]
**type_parameters** | [**\cbdesk\Mirakl\Model\PM11Response200AttributesTypeParameters[]**](PM11Response200AttributesTypeParameters.md) | Specificities of the attribute type, for example the date format, or the maximum size of a media | [optional]
**unique_code** | **string** | Unique code of the attribute | [optional]
**validations** | **string** | Validations applied to the attribute (a list of validations separated by commas) | [optional]
**values** | [**\cbdesk\Mirakl\Model\PM11Response200AttributesValues[]**](PM11Response200AttributesValues.md) | A list of authorized values for this attribute | [optional]
**values_list** | **string** | This code points to the list defining the authorized values for this attribute. | [optional]
**variant** | **bool** | Whether or not the attribute is a variation axis. Possible values: &lt;code&gt;true&lt;/code&gt; or &lt;code&gt;false&lt;/code&gt; | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
