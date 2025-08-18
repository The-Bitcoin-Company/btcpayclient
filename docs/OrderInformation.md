# OrderInformation

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**order_id** | Option<**String**> | Refers to the order ID from an external system, such as an e-commerce platform like WooCommerce. This property is indexed, allowing for efficient invoice searches using the `orderId`. | [optional]
**order_url** | Option<**String**> | Refers to a URL linking back to the order page of the external system. This link is displayed in the invoice details view. | [optional]
**tax_included** | Option<**f64**> | Represents the tax amount in the invoice currency. This information will appear in the invoice details view. During invoice creation, the value is automatically rounded to significant digits and ensured not to be greater than the invoice's price. | [optional]
**physical** | Option<**String**> | Indicates if this is a physical good; displayed in the invoice details view and in the BitPay API-compatible endpoints. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


