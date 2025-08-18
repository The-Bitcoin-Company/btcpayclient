# \InvoicesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**invoices_activate_payment_method**](InvoicesApi.md#invoices_activate_payment_method) | **POST** /api/v1/stores/{storeId}/invoices/{invoiceId}/payment-methods/{paymentMethodId}/activate | Activate Payment Method
[**invoices_archive_invoice**](InvoicesApi.md#invoices_archive_invoice) | **DELETE** /api/v1/stores/{storeId}/invoices/{invoiceId} | Archive invoice
[**invoices_create_invoice**](InvoicesApi.md#invoices_create_invoice) | **POST** /api/v1/stores/{storeId}/invoices | Create a new invoice
[**invoices_get_invoice**](InvoicesApi.md#invoices_get_invoice) | **GET** /api/v1/stores/{storeId}/invoices/{invoiceId} | Get invoice
[**invoices_get_invoice_payment_methods**](InvoicesApi.md#invoices_get_invoice_payment_methods) | **GET** /api/v1/stores/{storeId}/invoices/{invoiceId}/payment-methods | Get invoice payment methods
[**invoices_get_invoice_refund_trigger_data**](InvoicesApi.md#invoices_get_invoice_refund_trigger_data) | **GET** /api/v1/stores/{storeId}/invoices/{invoiceId}/refund/{paymentMethodId} | Get invoice refund trigger data
[**invoices_get_invoices**](InvoicesApi.md#invoices_get_invoices) | **GET** /api/v1/stores/{storeId}/invoices | Get invoices
[**invoices_mark_invoice_status**](InvoicesApi.md#invoices_mark_invoice_status) | **POST** /api/v1/stores/{storeId}/invoices/{invoiceId}/status | Mark invoice status
[**invoices_refund**](InvoicesApi.md#invoices_refund) | **POST** /api/v1/stores/{storeId}/invoices/{invoiceId}/refund | Refund invoice
[**invoices_unarchive_invoice**](InvoicesApi.md#invoices_unarchive_invoice) | **POST** /api/v1/stores/{storeId}/invoices/{invoiceId}/unarchive | Unarchive invoice
[**invoices_update_invoice**](InvoicesApi.md#invoices_update_invoice) | **PUT** /api/v1/stores/{storeId}/invoices/{invoiceId} | Update invoice



## invoices_activate_payment_method

> invoices_activate_payment_method(invoice_id, payment_method_id, store_id)
Activate Payment Method

Activate an invoice payment method (if lazy payments mode is enabled)

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**invoice_id** | **String** | The invoice ID | [required] |
**payment_method_id** | **String** | The payment method id of the payment method to update | [required] |
**store_id** | **String** | The store ID | [required] |

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## invoices_archive_invoice

> invoices_archive_invoice(invoice_id, store_id)
Archive invoice

Archives the specified invoice.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**invoice_id** | **String** | The invoice ID | [required] |
**store_id** | **String** | The store ID | [required] |

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## invoices_create_invoice

> models::InvoiceData invoices_create_invoice(store_id, create_invoice_request)
Create a new invoice

Create a new invoice

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |
**create_invoice_request** | [**CreateInvoiceRequest**](CreateInvoiceRequest.md) |  | [required] |

### Return type

[**models::InvoiceData**](InvoiceData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## invoices_get_invoice

> models::InvoiceData invoices_get_invoice(invoice_id, store_id)
Get invoice

View information about the specified invoice

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**invoice_id** | **String** | The invoice ID | [required] |
**store_id** | **String** | The store ID | [required] |

### Return type

[**models::InvoiceData**](InvoiceData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## invoices_get_invoice_payment_methods

> Vec<models::InvoicePaymentMethodDataModel> invoices_get_invoice_payment_methods(invoice_id, store_id, include_sensitive, only_accounted_payments)
Get invoice payment methods

View information about the specified invoice's payment methods

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**invoice_id** | **String** | The invoice ID | [required] |
**store_id** | **String** | The store ID | [required] |
**include_sensitive** | Option<**bool**> | If `true`, `additionalData` might include sensitive data (such as xpub). Requires the permission `btcpay.store.canmodifystoresettings`. |  |[default to false]
**only_accounted_payments** | Option<**bool**> | If default or true, only returns payments which are accounted (in Bitcoin, this mean not returning RBF'd or double spent payments) |  |[default to true]

### Return type

[**Vec<models::InvoicePaymentMethodDataModel>**](InvoicePaymentMethodDataModel.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## invoices_get_invoice_refund_trigger_data

> models::InvoiceRefundTriggerData invoices_get_invoice_refund_trigger_data(invoice_id, payment_method_id, store_id)
Get invoice refund trigger data

View calculated refund amounts (payment then/now, invoice, overpaid) for the specified invoice/payment-method. This can be used preceding the POST /refund call.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**invoice_id** | **String** | The invoice ID | [required] |
**payment_method_id** | **String** | The payment method id of the payment method to update | [required] |
**store_id** | **String** | The store ID | [required] |

### Return type

[**models::InvoiceRefundTriggerData**](InvoiceRefundTriggerData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## invoices_get_invoices

> Vec<models::InvoiceData> invoices_get_invoices(store_id, order_id, text_search, status, end_date, take, skip, start_date)
Get invoices

View information about the existing invoices

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |
**order_id** | Option<[**Vec<String>**](String.md)> | Array of OrderIds to fetch the invoices for |  |
**text_search** | Option<**String**> | A term that can help locating specific invoices. |  |
**status** | Option<[**InvoiceStatus**](.md)> | Array of statuses of invoices to be fetched |  |
**end_date** | Option<**f64**> | End date of the period to retrieve invoices |  |
**take** | Option<**f64**> | Number of records returned in response |  |
**skip** | Option<**f64**> | Number of records to skip |  |
**start_date** | Option<**f64**> | Start date of the period to retrieve invoices |  |

### Return type

[**Vec<models::InvoiceData>**](InvoiceData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## invoices_mark_invoice_status

> models::InvoiceData invoices_mark_invoice_status(invoice_id, store_id, mark_invoice_status_request)
Mark invoice status

Mark an invoice as invalid or settled.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**invoice_id** | **String** | The invoice ID | [required] |
**store_id** | **String** | The store ID | [required] |
**mark_invoice_status_request** | [**MarkInvoiceStatusRequest**](MarkInvoiceStatusRequest.md) |  | [required] |

### Return type

[**models::InvoiceData**](InvoiceData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## invoices_refund

> models::PullPaymentData invoices_refund(invoice_id, store_id, invoices_refund_request)
Refund invoice

Refund invoice

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**invoice_id** | **String** | The invoice ID | [required] |
**store_id** | **String** | The store ID | [required] |
**invoices_refund_request** | [**InvoicesRefundRequest**](InvoicesRefundRequest.md) |  | [required] |

### Return type

[**models::PullPaymentData**](PullPaymentData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## invoices_unarchive_invoice

> models::InvoiceData invoices_unarchive_invoice(invoice_id, store_id)
Unarchive invoice

Unarchive an invoice

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**invoice_id** | **String** | The invoice ID | [required] |
**store_id** | **String** | The store ID | [required] |

### Return type

[**models::InvoiceData**](InvoiceData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## invoices_update_invoice

> models::InvoiceData invoices_update_invoice(invoice_id, store_id, update_invoice_request)
Update invoice

Updates the specified invoice.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**invoice_id** | **String** | The invoice ID | [required] |
**store_id** | **String** | The store ID | [required] |
**update_invoice_request** | [**UpdateInvoiceRequest**](UpdateInvoiceRequest.md) |  | [required] |

### Return type

[**models::InvoiceData**](InvoiceData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

