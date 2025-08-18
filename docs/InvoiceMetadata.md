# InvoiceMetadata

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**buyer_name** | Option<**String**> | Visible in the invoice details view and in the BitPay API-compatible endpoints. | [optional]
**buyer_email** | Option<**String**> | Visible in the invoice details view and in the BitPay API-compatible endpoints. | [optional]
**buyer_country** | Option<**String**> | Visible in the invoice details view and in the BitPay API-compatible endpoints. | [optional]
**buyer_zip** | Option<**String**> | Visible in the invoice details view and in the BitPay API-compatible endpoints. | [optional]
**buyer_state** | Option<**String**> | Visible in the invoice details view and in the BitPay API-compatible endpoints. | [optional]
**buyer_city** | Option<**String**> | Visible in the invoice details view and in the BitPay API-compatible endpoints. | [optional]
**buyer_address1** | Option<**String**> | Visible in the invoice details view and in the BitPay API-compatible endpoints. | [optional]
**buyer_address2** | Option<**String**> | Visible in the invoice details view and in the BitPay API-compatible endpoints. | [optional]
**buyer_phone** | Option<**String**> | Visible in the invoice details view and in the BitPay API-compatible endpoints. | [optional]
**item_desc** | Option<**String**> | When using the Point of Sale (except in keypad or cart view), this field is set to the item description of the purchased item. This information is included in the CSV invoice export feature and appears in the invoice details view. | [optional]
**item_code** | Option<**String**> | When using the Point of Sale (except in keypad or cart view), this field is set to the item code of the purchased item. This information is included in the CSV invoice export feature and appears in the invoice details view. | [optional]
**order_id** | Option<**String**> | Refers to the order ID from an external system, such as an e-commerce platform like WooCommerce. This property is indexed, allowing for efficient invoice searches using the `orderId`. | [optional]
**order_url** | Option<**String**> | Refers to a URL linking back to the order page of the external system. This link is displayed in the invoice details view. | [optional]
**tax_included** | Option<**f64**> | Represents the tax amount in the invoice currency. This information will appear in the invoice details view. During invoice creation, the value is automatically rounded to significant digits and ensured not to be greater than the invoice's price. | [optional]
**physical** | Option<**String**> | Indicates if this is a physical good; displayed in the invoice details view and in the BitPay API-compatible endpoints. | [optional]
**payment_request_id** | Option<**String**> | In the invoice details view, a link is provided for navigating to the payment request page associated with the invoice. | [optional]
**pos_data** | Option<[**serde_json::Value**](.md)> | A custom JSON object that represents information displayed in the invoice details view. | [optional]
**receipt_data** | Option<[**serde_json::Value**](.md)> | A custom JSON object that represents information displayed on the receipt page of an invoice. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


