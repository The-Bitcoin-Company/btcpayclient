# CrowdfundBaseData

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
**enabled** | Option<**bool**> | Whether the app is enabled to be viewed by everyone | [optional]
**enforce_target_amount** | Option<**bool**> | Whether contributions over the set target amount are allowed | [optional]
**start_date** | Option<**f64**> | UNIX timestamp for crowdfund start time (https://www.unixtimestamp.com/) | [optional]
**end_date** | Option<**f64**> | UNIX timestamp for crowdfund end time (https://www.unixtimestamp.com/) | [optional]
**target_currency** | Option<**String**> | Target currency for the crowdfund | [optional]
**target_amount** | Option<**f64**> | Target amount for the crowdfund | [optional]
**main_image_url** | Option<**String**> | URL for image used as a cover image for the app | [optional]
**notification_url** | Option<**String**> | Callback notification url to POST to once when invoice is paid for and once when there are enough blockchain confirmations | [optional]
**tagline** | Option<**String**> | Tagline for the app displayed to user | [optional]
**disqus_enabled** | Option<**bool**> | Whether Disqus is enabled for the app | [optional]
**disqus_shortname** | Option<**String**> | Disqus shortname to used for the app | [optional]
**sounds_enabled** | Option<**bool**> | Whether sounds on new contributions are enabled | [optional]
**animations_enabled** | Option<**bool**> | Whether background animations on new contributions are enabled | [optional]
**reset_every_amount** | Option<**f64**> | Contribution goal reset frequency amount | [optional]
**reset_every** | Option<**String**> | Contribution goal reset frequency | [optional]
**display_perks_value** | Option<**bool**> | Whether perk values are displayed | [optional]
**sort_perks_by_popularity** | Option<**bool**> | Whether perks are sorted by popularity | [optional][default to true]
**sounds** | Option<**Vec<String>**> | Array of custom sounds which can be used on new contributions | [optional]
**animation_colors** | Option<**Vec<String>**> | Array of custom HEX colors which can be used for background animations on new contributions | [optional]
**html_lang** | Option<**String**> | Used for SEO, the [HTML Lang](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/lang) of the page | [optional]
**html_meta_tags** | Option<**String**> | Used for SEO, the [Meta tags](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/meta) of the page | [optional]
**form_id** | Option<**String**> | Form ID to request customer data | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


