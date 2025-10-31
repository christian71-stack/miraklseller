# # P11Response200ProductsOffers

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**active** | **bool** | Is the offer active | [optional]
**all_prices** | [**\cbdesk\Mirakl\Model\P11Response200ProductsOffersAllPrices[]**](P11Response200ProductsOffersAllPrices.md) | All prices for the offer &lt;br/&gt; For Dropship specifically: the list of purchasing prices of the offer, also referred to as costs or wholesale prices | [optional]
**allow_quote_requests** | **bool** | Whether the offer is eligible for quotation | [optional]
**applicable_pricing** | [**\cbdesk\Mirakl\Model\P11Response200ProductsOffersApplicablePricing**](P11Response200ProductsOffersApplicablePricing.md) |  | [optional]
**currency_iso_code** | **string** | The currency of the shop (iso format) | [optional]
**description** | **string** | Offer description | [optional]
**eco_contributions** | [**\cbdesk\Mirakl\Model\P11Response200ProductsOffersEcoContributions[]**](P11Response200ProductsOffersEcoContributions.md) | Eco-contributions of the offer - only available if the operator setting &lt;em&gt;Activate data collection related to circular economy regulations&lt;/em&gt; has been enabled. | [optional]
**inactivity_reasons** | **string[]** | Reasons for offers inactivity, mandatory if an offer is inactive | [optional]
**is_professional** | **bool** | Whether or not the shop is professional | [optional]
**leadtime_to_ship** | **int** | Offer&#39;s lead time to ship value. If this value has been set to 0, value is returned as 1 (unless platform&#39;s default lead time to ship value is also 0). If no lead time to ship was specified for the offer, platform&#39;s default value is returned. | [optional]
**min_shipping_price** | **float** | Unit price of the minimum shipping rate | [optional]
**min_shipping_price_additional** | **float** | Additional unit price associated to the minimum shipping rate | [optional]
**min_shipping_type** | **string** | Code of the shipping type associated to the minimum shipping rate | [optional]
**min_shipping_zone** | **string** | Code of the shipping zone associated to the minimum shipping rate | [optional]
**msrp** | **float** | The retail price recommendation, also referred to as manufacturer&#39;s suggested retail price (MSRP) or recommended retail price (RRP). &lt;br/&gt; Applicable only for Dropship offers. | [optional]
**nb_evaluation** | **int** | Number of customers evaluations | [optional]
**price** | **float** | Price of the offer &lt;br/&gt; For Dropship specifically: the purchasing price of the offer, also referred to as cost or wholesale price | [optional]
**price_additional_info** | **string** | Additional price information for the offer | [optional]
**retail_prices** | [**\cbdesk\Mirakl\Model\P11Response200ProductsOffersRetailPrices[]**](P11Response200ProductsOffersRetailPrices.md) | List retail prices for the offer, also referred to as selling prices. &lt;br/&gt; Applicable only for Dropship offers. | [optional]
**shipping_deadline** | **\DateTime** | Estimated shipping date, that includes business closing days and cut-off configured on the platform. Add the earliest and latest delivery times to calculate the estimated delivery date to customers | [optional]
**shipping_types** | [**\cbdesk\Mirakl\Model\P11Response200ProductsOffersShippingTypes[]**](P11Response200ProductsOffersShippingTypes.md) | List of shipping types compatible with the given offer | [optional]
**shop_grade** | **float** | Grade of the shop which proposes the offer | [optional]
**shop_name** | **string** | Name of the shop which proposes the offer | [optional]
**state_code** | **string** | Offer condition | [optional]
**total_price** | **float** | Total price of the offer (price + minimum shipping rate) &lt;br/&gt; For Dropship specifically: the purchasing price of the offer + minimum shipping rate | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
