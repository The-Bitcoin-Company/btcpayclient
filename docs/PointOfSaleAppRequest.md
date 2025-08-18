# PointOfSaleAppRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | Option<**String**> | Id of the app | [optional]
**app_name** | Option<**String**> | Name given to the app when it was created | [optional]
**store_id** | Option<**String**> | Id of the store to which the app belongs | [optional]
**created** | Option<**i32**> | UNIX timestamp for when the app was created | [optional]
**app_type** | Option<**String**> | Type of the app which was created | [optional]
**archived** | Option<**bool**> | If true, the app does not appear in the apps list by default. | [optional][default to false]
**title** | Option<**String**> | Display title of the app | [optional]
**description** | Option<**String**> | App description | [optional]
**default_view** | Option<**String**> | App view type (e.g., static, cart, etc...) | [optional]
**show_items** | Option<**bool**> | Display item selection for keypad | [optional][default to false]
**show_custom_amount** | Option<**bool**> | Whether the option to enter a custom amount is shown | [optional]
**show_discount** | Option<**bool**> | Whether the option to enter a discount is shown | [optional][default to false]
**show_search** | Option<**bool**> | Display the search bar | [optional][default to true]
**show_categories** | Option<**bool**> | Display the list of categories | [optional][default to true]
**enable_tips** | Option<**bool**> | Whether the option to enter a tip is shown | [optional][default to false]
**currency** | Option<**String**> | Currency used for the app | [optional]
**fixed_amount_pay_button_text** | Option<**String**> | Payment button text template for items with a set price | [optional]
**custom_amount_pay_button_text** | Option<**String**> | Payment button text which appears for items which allow user to input a custom amount | [optional]
**tip_text** | Option<**String**> | Prompt which appears next to the tip amount field if tipping is enabled | [optional]
**custom_tip_percentages** | Option<**Vec<f64>**> | Array of predefined tip percentage amounts | [optional][default to [15, 18, 20]]
**notification_url** | Option<**String**> | Callback notification url to POST to once when invoice is paid for and once when there are enough blockchain confirmations | [optional]
**redirect_url** | Option<**String**> | URL user is redirected to once invoice is paid | [optional]
**redirect_automatically** | Option<**bool**> | Whether user is redirected to specified redirect URL automatically after the invoice is paid | [optional]
**html_lang** | Option<**String**> | Used for SEO, the [HTML Lang](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/lang) of the page | [optional]
**html_meta_tags** | Option<**String**> | Used for SEO, the [Meta tags](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/meta) of the page | [optional]
**form_id** | Option<**String**> | Form ID to request customer data | [optional]
**template** | Option<**String**> | JSON of item available in the app | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


