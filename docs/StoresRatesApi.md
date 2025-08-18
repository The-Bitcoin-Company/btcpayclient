# \StoresRatesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**stores_get_store_rate_configuration**](StoresRatesApi.md#stores_get_store_rate_configuration) | **GET** /api/v1/stores/{storeId}/rates/configuration/{rateSource} | Get store rate settings for the specified rate source
[**stores_get_store_rates**](StoresRatesApi.md#stores_get_store_rates) | **GET** /api/v1/stores/{storeId}/rates | Get rates
[**stores_preview_store_rate_configuration**](StoresRatesApi.md#stores_preview_store_rate_configuration) | **POST** /api/v1/stores/{storeId}/rates/configuration/preview | Preview rate configuration results
[**stores_update_store_rate_configuration**](StoresRatesApi.md#stores_update_store_rate_configuration) | **PUT** /api/v1/stores/{storeId}/rates/configuration/{rateSource} | Get store rate settings for the specified rate source



## stores_get_store_rate_configuration

> models::StoreRateConfiguration stores_get_store_rate_configuration(rate_source, store_id)
Get store rate settings for the specified rate source

View rate settings for the specified store and rate source (`primary` or `fallback`).

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**rate_source** | **String** | The rate source to configure (`primary` or `fallback`) | [required] |[default to primary]
**store_id** | **String** | The store ID | [required] |

### Return type

[**models::StoreRateConfiguration**](StoreRateConfiguration.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## stores_get_store_rates

> Vec<models::StoreRateResult> stores_get_store_rates(store_id, currency_pair)
Get rates

Get rates on the store

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |
**currency_pair** | Option<[**Vec<String>**](String.md)> | The currency pairs to fetch rates for |  |

### Return type

[**Vec<models::StoreRateResult>**](StoreRateResult.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## stores_preview_store_rate_configuration

> Vec<models::StoreRateResult> stores_preview_store_rate_configuration(store_id, store_rate_configuration, currency_pair)
Preview rate configuration results

Preview rate configuration results before you set it on the store

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |
**store_rate_configuration** | [**StoreRateConfiguration**](StoreRateConfiguration.md) |  | [required] |
**currency_pair** | Option<[**Vec<String>**](String.md)> | The currency pairs to preview |  |

### Return type

[**Vec<models::StoreRateResult>**](StoreRateResult.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## stores_update_store_rate_configuration

> models::StoreRateConfiguration stores_update_store_rate_configuration(rate_source, store_id, store_rate_configuration)
Get store rate settings for the specified rate source

Update rate settings for the specified store and rate source (`primary` or `fallback`).

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**rate_source** | **String** | The rate source to configure (`primary` or `fallback`) | [required] |[default to primary]
**store_id** | **String** | The store ID | [required] |
**store_rate_configuration** | [**StoreRateConfiguration**](StoreRateConfiguration.md) |  | [required] |

### Return type

[**models::StoreRateConfiguration**](StoreRateConfiguration.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

