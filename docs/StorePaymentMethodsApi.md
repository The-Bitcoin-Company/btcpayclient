# \StorePaymentMethodsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**store_payment_methods_delete_store_payment_method**](StorePaymentMethodsApi.md#store_payment_methods_delete_store_payment_method) | **DELETE** /api/v1/stores/{storeId}/payment-methods/{paymentMethodId} | Delete store's payment method
[**store_payment_methods_get_store_payment_method**](StorePaymentMethodsApi.md#store_payment_methods_get_store_payment_method) | **GET** /api/v1/stores/{storeId}/payment-methods/{paymentMethodId} | Get store payment method
[**store_payment_methods_get_store_payment_methods**](StorePaymentMethodsApi.md#store_payment_methods_get_store_payment_methods) | **GET** /api/v1/stores/{storeId}/payment-methods | Get store payment methods
[**store_payment_methods_update_store_payment_method**](StorePaymentMethodsApi.md#store_payment_methods_update_store_payment_method) | **PUT** /api/v1/stores/{storeId}/payment-methods/{paymentMethodId} | Update store's payment method



## store_payment_methods_delete_store_payment_method

> store_payment_methods_delete_store_payment_method(payment_method_id, store_id)
Delete store's payment method

Delete information about the stores' configured payment method

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
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


## store_payment_methods_get_store_payment_method

> models::GenericPaymentMethodData store_payment_methods_get_store_payment_method(payment_method_id, store_id, include_config)
Get store payment method

View information about the stores' configured payment method

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**payment_method_id** | **String** | The payment method id of the payment method to update | [required] |
**store_id** | **String** | The store ID | [required] |
**include_config** | Option<**bool**> | Fetch the config of the payment methods, if `true`, the permission `btcpay.store.canmodifystoresettings` is required. |  |

### Return type

[**models::GenericPaymentMethodData**](GenericPaymentMethodData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_payment_methods_get_store_payment_methods

> Vec<models::GenericPaymentMethodData> store_payment_methods_get_store_payment_methods(store_id, only_enabled, include_config)
Get store payment methods

View information about the stores' configured payment methods

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |
**only_enabled** | Option<**bool**> | Fetch payment methods that are enabled/disabled only |  |
**include_config** | Option<**bool**> | Fetch the config of the payment methods, if `true`, the permission `btcpay.store.canmodifystoresettings` is required. |  |

### Return type

[**Vec<models::GenericPaymentMethodData>**](GenericPaymentMethodData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_payment_methods_update_store_payment_method

> models::GenericPaymentMethodData store_payment_methods_update_store_payment_method(payment_method_id, store_id, update_payment_method_config)
Update store's payment method

Update information about the stores' configured payment method

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**payment_method_id** | **String** | The payment method id of the payment method to update | [required] |
**store_id** | **String** | The store ID | [required] |
**update_payment_method_config** | Option<[**UpdatePaymentMethodConfig**](UpdatePaymentMethodConfig.md)> |  |  |

### Return type

[**models::GenericPaymentMethodData**](GenericPaymentMethodData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

