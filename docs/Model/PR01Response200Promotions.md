# # PR01Response200Promotions

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount_off** | **float** | The amount off of the promotion. &lt;br/&gt;Only applicable when promotion is of type &lt;code&gt;AMOUNT_OFF&lt;/code&gt;, null otherwise | [optional]
**application_to_cart** | [**\cbdesk\Mirakl\Model\PR01Response200PromotionsApplicationToCart[]**](PR01Response200PromotionsApplicationToCart.md) | If applicable, returns promo code associated to the promotion | [optional]
**campaign** | [**\cbdesk\Mirakl\Model\PR01Response200PromotionsCampaign**](PR01Response200PromotionsCampaign.md) |  | [optional]
**channels** | [**\cbdesk\Mirakl\Model\PR01Response200PromotionsChannels[]**](PR01Response200PromotionsChannels.md) | Channels on which the promotion is applied. If none, promotion applied on all channels | [optional]
**customer_group_ids** | **string[]** | The customer groups on which the promotion is applied. If none, promotion applies to all customer groups. | [optional]
**customer_organization_ids** | **string[]** | The customer organizations on which the promotion is applied. If none, promotion applies to all customer organizations. | [optional]
**date_created** | **\DateTime** | Creation date of the promotion | [optional]
**end_date** | **\DateTime** | End date of the promotion period of activity | [optional]
**free_items_quantity** | **int** | The free item target quantity of the promotion. &lt;br/&gt;Only applicable when promotion is of type &lt;code&gt;FREE_ITEMS&lt;/code&gt;, null otherwise | [optional]
**internal_description** | **string** | Internal description of the promotion, set by the shop | [optional]
**internal_id** | **string** | Promotion identifier | [optional]
**last_updated** | **\DateTime** | Last update date of the promotion | [optional]
**max_quantity_to_discount** | **int** | Maximum quantity of items on which a percentage off discount applies. Only applicable when promotion is of type PERCENTAGE_OFF, null otherwise | [optional]
**medias** | [**\cbdesk\Mirakl\Model\PR01Response200PromotionsMedias[]**](PR01Response200PromotionsMedias.md) | The medias associated with this promotion, with the locales they apply to | [optional]
**percentage_off** | **float** | The percentage off of the promotion. &lt;br/&gt;Only applicable when promotion is of type &lt;code&gt;PERCENTAGE_OFF&lt;/code&gt;, null otherwise | [optional]
**public_descriptions** | [**\cbdesk\Mirakl\Model\PR01Response200PromotionsPublicDescriptions[]**](PR01Response200PromotionsPublicDescriptions.md) | The public descriptions of the promotion, with the locales they apply to | [optional]
**reduced_unit_price** | **float** | The new offer’s unit price triggered by the promotion. &lt;br/&gt;Only applicable when promotion is of type &lt;code&gt;REDUCED_UNIT_PRICE&lt;/code&gt;, null otherwise. | [optional]
**reward_offer_ids** | **int[]** | Offers used as reward in the promotion, according to the requested reward_offer_ids | [optional]
**reward_on_purchased_items** | **bool** | Specifies if the promotion&#39;s reward applies to purchased items or to a specific selection | [optional]
**start_date** | **\DateTime** | Start date of the promotion period of activity | [optional]
**state** | **string** | Promotion state | [optional]
**trigger_offer_ids** | **int[]** | Offers which trigger the promotion, according to the requested trigger_offer_ids | [optional]
**triggers** | [**\cbdesk\Mirakl\Model\PR01Response200PromotionsTriggers[]**](PR01Response200PromotionsTriggers.md) | Triggers of the promotion | [optional]
**type** | **string** | Promotion type | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
