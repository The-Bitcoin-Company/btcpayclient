# \LightningInternalNodeApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**internal_lightning_node_api_connect_to_node**](LightningInternalNodeApi.md#internal_lightning_node_api_connect_to_node) | **POST** /api/v1/server/lightning/{cryptoCode}/connect | Connect to lightning node
[**internal_lightning_node_api_create_invoice**](LightningInternalNodeApi.md#internal_lightning_node_api_create_invoice) | **POST** /api/v1/server/lightning/{cryptoCode}/invoices | Create lightning invoice
[**internal_lightning_node_api_get_balance**](LightningInternalNodeApi.md#internal_lightning_node_api_get_balance) | **GET** /api/v1/server/lightning/{cryptoCode}/balance | Get node balance
[**internal_lightning_node_api_get_channels**](LightningInternalNodeApi.md#internal_lightning_node_api_get_channels) | **GET** /api/v1/server/lightning/{cryptoCode}/channels | Get channels
[**internal_lightning_node_api_get_deposit_address**](LightningInternalNodeApi.md#internal_lightning_node_api_get_deposit_address) | **POST** /api/v1/server/lightning/{cryptoCode}/address | Get deposit address
[**internal_lightning_node_api_get_histogram**](LightningInternalNodeApi.md#internal_lightning_node_api_get_histogram) | **GET** /api/v1/server/lightning/{cryptoCode}/histogram | Get node balance histogram
[**internal_lightning_node_api_get_info**](LightningInternalNodeApi.md#internal_lightning_node_api_get_info) | **GET** /api/v1/server/lightning/{cryptoCode}/info | Get node information
[**internal_lightning_node_api_get_invoice**](LightningInternalNodeApi.md#internal_lightning_node_api_get_invoice) | **GET** /api/v1/server/lightning/{cryptoCode}/invoices/{id} | Get invoice
[**internal_lightning_node_api_get_invoices**](LightningInternalNodeApi.md#internal_lightning_node_api_get_invoices) | **GET** /api/v1/server/lightning/{cryptoCode}/invoices | Get invoices
[**internal_lightning_node_api_get_payment**](LightningInternalNodeApi.md#internal_lightning_node_api_get_payment) | **GET** /api/v1/server/lightning/{cryptoCode}/payments/{paymentHash} | Get payment
[**internal_lightning_node_api_get_payments**](LightningInternalNodeApi.md#internal_lightning_node_api_get_payments) | **GET** /api/v1/server/lightning/{cryptoCode}/payments | Get payments
[**internal_lightning_node_api_open_channel**](LightningInternalNodeApi.md#internal_lightning_node_api_open_channel) | **POST** /api/v1/server/lightning/{cryptoCode}/channels | Open channel
[**internal_lightning_node_api_pay_invoice**](LightningInternalNodeApi.md#internal_lightning_node_api_pay_invoice) | **POST** /api/v1/server/lightning/{cryptoCode}/invoices/pay | Pay Lightning Invoice



## internal_lightning_node_api_connect_to_node

> internal_lightning_node_api_connect_to_node(crypto_code, connect_to_node_request)
Connect to lightning node

Connect to another lightning node.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**crypto_code** | **String** | The cryptoCode of the lightning-node to query | [required] |
**connect_to_node_request** | [**ConnectToNodeRequest**](ConnectToNodeRequest.md) |  | [required] |

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## internal_lightning_node_api_create_invoice

> models::LightningInvoiceData internal_lightning_node_api_create_invoice(crypto_code, create_lightning_invoice_request)
Create lightning invoice

Create a lightning invoice.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**crypto_code** | **String** | The cryptoCode of the lightning-node to query | [required] |
**create_lightning_invoice_request** | [**CreateLightningInvoiceRequest**](CreateLightningInvoiceRequest.md) |  | [required] |

### Return type

[**models::LightningInvoiceData**](LightningInvoiceData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## internal_lightning_node_api_get_balance

> models::LightningNodeBalanceData internal_lightning_node_api_get_balance(crypto_code)
Get node balance

View balance of the lightning node

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**crypto_code** | **String** | The cryptoCode of the lightning-node to query | [required] |

### Return type

[**models::LightningNodeBalanceData**](LightningNodeBalanceData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## internal_lightning_node_api_get_channels

> Vec<models::LightningChannelData> internal_lightning_node_api_get_channels(crypto_code)
Get channels

View information about the current channels of the lightning node

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**crypto_code** | **String** | The cryptoCode of the lightning-node to query | [required] |

### Return type

[**Vec<models::LightningChannelData>**](LightningChannelData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## internal_lightning_node_api_get_deposit_address

> String internal_lightning_node_api_get_deposit_address(crypto_code)
Get deposit address

Get an on-chain deposit address for the lightning node 

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**crypto_code** | **String** | The cryptoCode of the lightning-node to query | [required] |

### Return type

**String**

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## internal_lightning_node_api_get_histogram

> models::HistogramData internal_lightning_node_api_get_histogram(crypto_code)
Get node balance histogram

View balance histogram of the lightning node

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**crypto_code** | **String** | The cryptoCode of the lightning-node to query | [required] |

### Return type

[**models::HistogramData**](HistogramData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## internal_lightning_node_api_get_info

> models::LightningNodeInformationData internal_lightning_node_api_get_info(crypto_code)
Get node information

View information about the lightning node

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**crypto_code** | **String** | The cryptoCode of the lightning-node to query | [required] |

### Return type

[**models::LightningNodeInformationData**](LightningNodeInformationData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## internal_lightning_node_api_get_invoice

> models::LightningInvoiceData internal_lightning_node_api_get_invoice(crypto_code, id)
Get invoice

View information about the requested lightning invoice

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**crypto_code** | **String** | The cryptoCode of the lightning-node to query | [required] |
**id** | **String** | The id of the lightning invoice. | [required] |

### Return type

[**models::LightningInvoiceData**](LightningInvoiceData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## internal_lightning_node_api_get_invoices

> Vec<models::LightningInvoiceData> internal_lightning_node_api_get_invoices(crypto_code, pending_only, offset_index)
Get invoices

View information about the lightning invoices

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**crypto_code** | **String** | The cryptoCode of the lightning-node to query | [required] |
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


## internal_lightning_node_api_get_payment

> models::LightningPaymentData internal_lightning_node_api_get_payment(crypto_code, payment_hash)
Get payment

View information about the requested lightning payment

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**crypto_code** | **String** | The cryptoCode of the lightning-node to query | [required] |
**payment_hash** | **String** | The payment hash of the lightning payment. | [required] |

### Return type

[**models::LightningPaymentData**](LightningPaymentData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## internal_lightning_node_api_get_payments

> Vec<models::LightningPaymentData> internal_lightning_node_api_get_payments(crypto_code, include_pending, offset_index)
Get payments

View information about the lightning payments

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**crypto_code** | **String** | The cryptoCode of the lightning-node to query | [required] |
**include_pending** | Option<**bool**> | Also include pending payments |  |[default to false]
**offset_index** | Option<**f64**> | The index of a payment that will be used as the start of the list |  |[default to 0]

### Return type

[**Vec<models::LightningPaymentData>**](LightningPaymentData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## internal_lightning_node_api_open_channel

> internal_lightning_node_api_open_channel(crypto_code, open_lightning_channel_request)
Open channel

Open a channel with another lightning node. You should connect to that node first.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**crypto_code** | **String** | The cryptoCode of the lightning-node to query | [required] |
**open_lightning_channel_request** | [**OpenLightningChannelRequest**](OpenLightningChannelRequest.md) |  | [required] |

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## internal_lightning_node_api_pay_invoice

> models::LightningPaymentData internal_lightning_node_api_pay_invoice(crypto_code, pay_lightning_invoice_request)
Pay Lightning Invoice

Pay a lightning invoice. In case the payment response times out, the status will be reported as pending and the final status can be resolved using the [Get payment](#operation/InternalLightningNodeApi_GetPayment) endpoint. The default wait time for payment responses is 30 seconds — it might take longer if multiple routes are tried or a hold invoice is getting paid.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**crypto_code** | **String** | The cryptoCode of the lightning-node to query | [required] |
**pay_lightning_invoice_request** | [**PayLightningInvoiceRequest**](PayLightningInvoiceRequest.md) |  | [required] |

### Return type

[**models::LightningPaymentData**](LightningPaymentData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

