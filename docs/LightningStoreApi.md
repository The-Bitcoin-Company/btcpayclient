# \LightningStoreApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**store_lightning_node_api_connect_to_node**](LightningStoreApi.md#store_lightning_node_api_connect_to_node) | **POST** /api/v1/stores/{storeId}/lightning/{cryptoCode}/connect | Connect to lightning node
[**store_lightning_node_api_create_invoice**](LightningStoreApi.md#store_lightning_node_api_create_invoice) | **POST** /api/v1/stores/{storeId}/lightning/{cryptoCode}/invoices | Create lightning invoice
[**store_lightning_node_api_get_balance**](LightningStoreApi.md#store_lightning_node_api_get_balance) | **GET** /api/v1/stores/{storeId}/lightning/{cryptoCode}/balance | Get node balance
[**store_lightning_node_api_get_channels**](LightningStoreApi.md#store_lightning_node_api_get_channels) | **GET** /api/v1/stores/{storeId}/lightning/{cryptoCode}/channels | Get channels
[**store_lightning_node_api_get_deposit_address**](LightningStoreApi.md#store_lightning_node_api_get_deposit_address) | **POST** /api/v1/stores/{storeId}/lightning/{cryptoCode}/address | Get deposit address
[**store_lightning_node_api_get_histogram**](LightningStoreApi.md#store_lightning_node_api_get_histogram) | **GET** /api/v1/stores/{storeId}/lightning/{cryptoCode}/histogram | Get node balance histogram
[**store_lightning_node_api_get_info**](LightningStoreApi.md#store_lightning_node_api_get_info) | **GET** /api/v1/stores/{storeId}/lightning/{cryptoCode}/info | Get node information
[**store_lightning_node_api_get_invoice**](LightningStoreApi.md#store_lightning_node_api_get_invoice) | **GET** /api/v1/stores/{storeId}/lightning/{cryptoCode}/invoices/{id} | Get invoice
[**store_lightning_node_api_get_invoices**](LightningStoreApi.md#store_lightning_node_api_get_invoices) | **GET** /api/v1/stores/{storeId}/lightning/{cryptoCode}/invoices | Get invoices
[**store_lightning_node_api_get_payment**](LightningStoreApi.md#store_lightning_node_api_get_payment) | **GET** /api/v1/stores/{storeId}/lightning/{cryptoCode}/payments/{paymentHash} | Get payment
[**store_lightning_node_api_get_payments**](LightningStoreApi.md#store_lightning_node_api_get_payments) | **GET** /api/v1/stores/{storeId}/lightning/{cryptoCode}/payments | Get payments
[**store_lightning_node_api_open_channel**](LightningStoreApi.md#store_lightning_node_api_open_channel) | **POST** /api/v1/stores/{storeId}/lightning/{cryptoCode}/channels | Open channel
[**store_lightning_node_api_pay_invoice**](LightningStoreApi.md#store_lightning_node_api_pay_invoice) | **POST** /api/v1/stores/{storeId}/lightning/{cryptoCode}/invoices/pay | Pay Lightning Invoice



## store_lightning_node_api_connect_to_node

> store_lightning_node_api_connect_to_node(crypto_code, store_id, connect_to_node_request)
Connect to lightning node

Connect to another lightning node.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**crypto_code** | **String** | The cryptoCode of the lightning-node to query | [required] |
**store_id** | **String** | The store ID | [required] |
**connect_to_node_request** | [**ConnectToNodeRequest**](ConnectToNodeRequest.md) |  | [required] |

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_lightning_node_api_create_invoice

> models::LightningInvoiceData store_lightning_node_api_create_invoice(crypto_code, store_id, create_lightning_invoice_request)
Create lightning invoice

Create a lightning invoice.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**crypto_code** | **String** | The cryptoCode of the lightning-node to query | [required] |
**store_id** | **String** | The store ID | [required] |
**create_lightning_invoice_request** | [**CreateLightningInvoiceRequest**](CreateLightningInvoiceRequest.md) |  | [required] |

### Return type

[**models::LightningInvoiceData**](LightningInvoiceData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_lightning_node_api_get_balance

> models::LightningNodeBalanceData store_lightning_node_api_get_balance(crypto_code, store_id)
Get node balance

View balance of the lightning node

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**crypto_code** | **String** | The cryptoCode of the lightning-node to query | [required] |
**store_id** | **String** | The store ID | [required] |

### Return type

[**models::LightningNodeBalanceData**](LightningNodeBalanceData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_lightning_node_api_get_channels

> Vec<models::LightningChannelData> store_lightning_node_api_get_channels(crypto_code, store_id)
Get channels

View information about the current channels of the lightning node

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**crypto_code** | **String** | The cryptoCode of the lightning-node to query | [required] |
**store_id** | **String** | The store ID | [required] |

### Return type

[**Vec<models::LightningChannelData>**](LightningChannelData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_lightning_node_api_get_deposit_address

> String store_lightning_node_api_get_deposit_address(store_id, crypto_code)
Get deposit address

Get an on-chain deposit address for the lightning node 

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |
**crypto_code** | **String** | The cryptoCode of the lightning-node to query | [required] |

### Return type

**String**

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_lightning_node_api_get_histogram

> models::HistogramData store_lightning_node_api_get_histogram(crypto_code, store_id)
Get node balance histogram

View balance histogram of the lightning node

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**crypto_code** | **String** | The cryptoCode of the lightning-node to query | [required] |
**store_id** | **String** | The store ID | [required] |

### Return type

[**models::HistogramData**](HistogramData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_lightning_node_api_get_info

> models::LightningNodeInformationData store_lightning_node_api_get_info(crypto_code, store_id)
Get node information

View information about the lightning node

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**crypto_code** | **String** | The cryptoCode of the lightning-node to query | [required] |
**store_id** | **String** | The store ID | [required] |

### Return type

[**models::LightningNodeInformationData**](LightningNodeInformationData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_lightning_node_api_get_invoice

> models::LightningInvoiceData store_lightning_node_api_get_invoice(crypto_code, store_id, id)
Get invoice

View information about the requested lightning invoice

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**crypto_code** | **String** | The cryptoCode of the lightning-node to query | [required] |
**store_id** | **String** | The store ID | [required] |
**id** | **String** | The id of the lightning invoice. | [required] |

### Return type

[**models::LightningInvoiceData**](LightningInvoiceData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_lightning_node_api_get_invoices

> Vec<models::LightningInvoiceData> store_lightning_node_api_get_invoices(crypto_code, store_id, pending_only, offset_index)
Get invoices

View information about the lightning invoices

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**crypto_code** | **String** | The cryptoCode of the lightning-node to query | [required] |
**store_id** | **String** | The store ID | [required] |
**pending_only** | Option<**bool**> | Limit to pending invoices only |  |[default to false]
**offset_index** | Option<**f64**> | The index of an invoice that will be used as the start of the list |  |[default to 0]

### Return type

[**Vec<models::LightningInvoiceData>**](LightningInvoiceData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_lightning_node_api_get_payment

> models::LightningPaymentData store_lightning_node_api_get_payment(crypto_code, store_id, payment_hash)
Get payment

View information about the requested lightning payment

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**crypto_code** | **String** | The cryptoCode of the lightning-node to query | [required] |
**store_id** | **String** | The store ID | [required] |
**payment_hash** | **String** | The payment hash of the lightning payment. | [required] |

### Return type

[**models::LightningPaymentData**](LightningPaymentData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_lightning_node_api_get_payments

> Vec<models::LightningPaymentData> store_lightning_node_api_get_payments(crypto_code, store_id, include_pending, offset_index)
Get payments

View information about the lightning payments

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**crypto_code** | **String** | The cryptoCode of the lightning-node to query | [required] |
**store_id** | **String** | The store ID | [required] |
**include_pending** | Option<**bool**> | Also include pending payments |  |[default to false]
**offset_index** | Option<**f64**> | The index of an invoice that will be used as the start of the list |  |[default to 0]

### Return type

[**Vec<models::LightningPaymentData>**](LightningPaymentData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_lightning_node_api_open_channel

> store_lightning_node_api_open_channel(crypto_code, store_id, open_lightning_channel_request)
Open channel

Open a channel with another lightning node. You should connect to that node first.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**crypto_code** | **String** | The cryptoCode of the lightning-node to query | [required] |
**store_id** | **String** | The store ID | [required] |
**open_lightning_channel_request** | [**OpenLightningChannelRequest**](OpenLightningChannelRequest.md) |  | [required] |

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_lightning_node_api_pay_invoice

> models::LightningPaymentData store_lightning_node_api_pay_invoice(crypto_code, store_id, pay_lightning_invoice_request)
Pay Lightning Invoice

Pay a lightning invoice. In case the payment response times out, the status will be reported as pending and the final status can be resolved using the [Get payment](#operation/StoreLightningNodeApi_GetPayment) endpoint. The default wait time for payment responses is 30 seconds — it might take longer if multiple routes are tried or a hold invoice is getting paid.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**crypto_code** | **String** | The cryptoCode of the lightning-node to query | [required] |
**store_id** | **String** | The store ID | [required] |
**pay_lightning_invoice_request** | [**PayLightningInvoiceRequest**](PayLightningInvoiceRequest.md) |  | [required] |

### Return type

[**models::LightningPaymentData**](LightningPaymentData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

