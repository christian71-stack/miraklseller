# # M11Response200Data

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**authorized_participants** | [**\cbdesk\Mirakl\Model\M11Response200DataAuthorizedParticipants[]**](M11Response200DataAuthorizedParticipants.md) | Thread authorized participants&lt;br/&gt; Those are the participants who are authorized to join the thread. | [optional]
**current_participants** | [**\cbdesk\Mirakl\Model\M11Response200DataCurrentParticipants[]**](M11Response200DataCurrentParticipants.md) | Thread current participants&lt;br/&gt; Those are the participants who have actually participated in the thread, meaning that they are either sender or receivers of at least one message of the thread.&lt;br/&gt; These participants must be on the list of the &lt;code&gt;authorized_participants&lt;/code&gt; | [optional]
**customer_organization** | [**\cbdesk\Mirakl\Model\M11Response200DataCustomerOrganization**](M11Response200DataCustomerOrganization.md) |  | [optional]
**date_created** | **\DateTime** | Thread created date | [optional]
**date_updated** | **\DateTime** | Thread updated date | [optional]
**entities** | [**\cbdesk\Mirakl\Model\M11Response200DataEntities[]**](M11Response200DataEntities.md) | Thread entities | [optional]
**id** | **string** | Thread id | [optional]
**messages** | [**\cbdesk\Mirakl\Model\M11Response200DataMessages[]**](M11Response200DataMessages.md) | Thread messages. Limited to the last 100 messages of the thread. Present if with_messages query parameter has been set to true | [optional]
**metadata** | [**\cbdesk\Mirakl\Model\M11Response200DataMetadata**](M11Response200DataMetadata.md) |  | [optional]
**no_store_reply_needed** | [**\cbdesk\Mirakl\Model\M11Response200DataNoStoreReplyNeeded[]**](M11Response200DataNoStoreReplyNeeded.md) | Thread \&quot;no store reply needed\&quot; actions. Present if \&quot;with_messages\&quot; query parameter has been set to true. | [optional]
**topic** | [**\cbdesk\Mirakl\Model\M11Response200DataTopic**](M11Response200DataTopic.md) |  | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
