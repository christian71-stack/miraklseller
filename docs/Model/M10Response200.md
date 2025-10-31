# # M10Response200

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**authorized_participants** | [**\cbdesk\Mirakl\Model\M10Response200AuthorizedParticipants[]**](M10Response200AuthorizedParticipants.md) | Thread authorized participants&lt;br/&gt; Those are the participants who are authorized to join the thread. | [optional]
**current_participants** | [**\cbdesk\Mirakl\Model\M10Response200CurrentParticipants[]**](M10Response200CurrentParticipants.md) | Thread current participants&lt;br/&gt; Those are the participants who have actually participated in the thread, meaning that they are either sender or receivers of at least one message of the thread.&lt;br/&gt; These participants must be on the list of the &lt;code&gt;authorized_participants&lt;/code&gt; | [optional]
**customer_organization** | [**\cbdesk\Mirakl\Model\M10Response200CustomerOrganization**](M10Response200CustomerOrganization.md) |  | [optional]
**date_created** | **\DateTime** | Thread created date | [optional]
**date_updated** | **\DateTime** | Thread updated date | [optional]
**entities** | [**\cbdesk\Mirakl\Model\M10Response200Entities[]**](M10Response200Entities.md) | Thread entities | [optional]
**id** | **string** | Thread id | [optional]
**messages** | [**\cbdesk\Mirakl\Model\M10Response200Messages[]**](M10Response200Messages.md) | Thread messages | [optional]
**metadata** | [**\cbdesk\Mirakl\Model\M10Response200Metadata**](M10Response200Metadata.md) |  | [optional]
**no_store_reply_needed** | [**\cbdesk\Mirakl\Model\M10Response200NoStoreReplyNeeded[]**](M10Response200NoStoreReplyNeeded.md) | Thread \&quot;no store reply needed\&quot; actions. | [optional]
**topic** | [**\cbdesk\Mirakl\Model\M10Response200Topic**](M10Response200Topic.md) |  | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
