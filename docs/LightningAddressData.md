# LightningAddressData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**username** | Option<**String**> | The username of the lightning address | [optional]
**currency_code** | Option<**String**> | The currency to generate the invoices for this lightning address in. Leave null lto use the store default. | [optional]
**min** | Option<**String**> | The minimum amount in sats this ln address allows | [optional]
**max** | Option<**String**> | The maximum amount in sats this ln address allows | [optional]
**invoice_metadata** | Option<[**serde_json::Value**](.md)> | The invoice metadata as JSON. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


