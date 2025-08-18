# StoreBaseData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | Option<**String**> | The name of the store | [optional]
**website** | Option<**String**> | The absolute url of the store | [optional]
**support_url** | Option<**String**> | The support URI of the store, can contain the placeholders `{OrderId}` and `{InvoiceId}`. Can be any valid URI, such as a website, email, and nostr. | [optional]
**logo_url** | Option<**String**> | Absolute URL to a logo file or a reference to an uploaded file id with `fileid:ID` | [optional]
**css_url** | Option<**String**> | Absolute URL to CSS file to customize the public/customer-facing pages of the store. (Invoice, Payment Request, Pull Payment, etc.) or a reference to an uploaded file id with `fileid:ID` | [optional]
**payment_sound_url** | Option<**String**> | Absolute URL to a sound file or a reference to an uploaded file id with `fileid:ID` | [optional]
**brand_color** | Option<**String**> | The brand color of the store in HEX format | [optional]
**apply_brand_color_to_backend** | Option<**bool**> | Apply the brand color to the store's backend as well | [optional][default to false]
**default_currency** | Option<**String**> | The default currency of the store | [optional][default to USD]
**additional_tracked_rates** | Option<**Vec<String>**> | Additional rates to track. The rates of those currencies, in addition to the default currency, will be recorded when a new invoice is created. The rates will then be accessible through reports. | [optional][default to []]
**invoice_expiration** | Option<[**models::TimeSpanSeconds**](serde_json::Value.md)> | The time after which an invoice is considered expired if not paid. The value will be rounded down to a minute. | [optional][default to 900]
**refund_bolt11_expiration** | Option<[**models::TimeSpanDays**](serde_json::Value.md)> | The minimum expiry of BOLT11 invoices accepted for refunds by default. (in days) | [optional][default to 30]
**display_expiration_timer** | Option<[**models::TimeSpanSeconds**](serde_json::Value.md)> | The time left that will trigger the countdown timer on the checkout page to be shown. The value will be rounded down to a minute. | [optional][default to 300]
**monitoring_expiration** | Option<[**models::TimeSpanSeconds**](serde_json::Value.md)> | The time after which an invoice which has been paid but not confirmed will be considered invalid. The value will be rounded down to a minute. | [optional][default to 86400]
**speed_policy** | Option<[**models::SpeedPolicy**](SpeedPolicy.md)> |  | [optional]
**lightning_description_template** | Option<**String**> | The BOLT11 description of the lightning invoice in the checkout. You can use placeholders '{StoreName}', '{ItemDescription}' and '{OrderId}'. | [optional]
**payment_tolerance** | Option<**f64**> | Consider an invoice fully paid, even if the payment is missing 'x' % of the full amount. | [optional][default to 0.0]
**archived** | Option<**bool**> | If true, the store does not appear in the stores list by default. | [optional][default to false]
**anyone_can_create_invoice** | Option<**bool**> | If true, then no authentication is needed to create invoices on this store. | [optional][default to false]
**receipt** | Option<[**models::ReceiptOptions**](ReceiptOptions.md)> | Additional settings to customize the public receipt | [optional]
**lightning_amount_in_satoshi** | Option<**bool**> | If true, lightning payment methods show amount in satoshi in the checkout page. | [optional][default to false]
**lightning_private_route_hints** | Option<**bool**> | Should private route hints be included in the lightning payment of the checkout page. | [optional][default to false]
**on_chain_with_ln_invoice_fallback** | Option<**bool**> | Unify on-chain and lightning payment URL. | [optional][default to false]
**redirect_automatically** | Option<**bool**> | After successfull payment, should the checkout page redirect the user automatically to the redirect URL of the invoice? | [optional][default to false]
**show_recommended_fee** | Option<**bool**> |  | [optional][default to true]
**recommended_fee_block_target** | Option<**i32**> | The fee rate recommendation in the checkout page for the on-chain payment to be confirmed after 'x' blocks. | [optional][default to 1]
**default_lang** | Option<**String**> | The default language to use in the checkout page. (The different translations available are listed [here](https://github.com/btcpayserver/btcpayserver/tree/master/BTCPayServer/wwwroot/locales) | [optional][default to en]
**html_title** | Option<**String**> | The HTML title of the checkout page (when you over the tab in your browser) | [optional]
**network_fee_mode** | Option<[**models::NetworkFeeMode**](NetworkFeeMode.md)> |  | [optional]
**pay_join_enabled** | Option<**bool**> | If true, payjoin will be proposed in the checkout page if possible. ([More information](https://docs.btcpayserver.org/Payjoin/)) | [optional][default to false]
**auto_detect_language** | Option<**bool**> | If true, the language on the checkout page will adapt to the language defined by the user's browser settings | [optional][default to false]
**show_pay_in_wallet_button** | Option<**bool**> | If true, the \"Pay in wallet\" button will be shown on the checkout page (Checkout V2) | [optional][default to true]
**show_store_header** | Option<**bool**> | If true, the store header will be shown on the checkout page (Checkout V2) | [optional][default to true]
**celebrate_payment** | Option<**bool**> | If true, payments on the checkout page will be celebrated with confetti (Checkout V2) | [optional][default to true]
**play_sound_on_payment** | Option<**bool**> | If true, sounds on the checkout page will be enabled (Checkout V2) | [optional][default to false]
**lazy_payment_methods** | Option<**bool**> | If true, payment methods are enabled individually upon user interaction in the invoice | [optional][default to false]
**default_payment_method** | Option<**String**> | Payment method IDs. Available payment method IDs for Bitcoin are:   - `\"BTC-CHAIN\"`: Onchain    -`\"BTC-LN\"`: Lightning    - `\"BTC-LNURL\"`: LNURL | [optional]
**payment_method_criteria** | Option<[**Vec<models::PaymentMethodCriteriaData>**](PaymentMethodCriteriaData.md)> | The criteria required to activate specific payment methods. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


