# \LightningAddressApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**store_lightning_addresses_add_or_update_store_lightning_address**](LightningAddressApi.md#store_lightning_addresses_add_or_update_store_lightning_address) | **POST** /api/v1/stores/{storeId}/lightning-addresses/{username} | Add or update store configured lightning address
[**store_lightning_addresses_get_store_lightning_address**](LightningAddressApi.md#store_lightning_addresses_get_store_lightning_address) | **GET** /api/v1/stores/{storeId}/lightning-addresses/{username} | Get store configured lightning address
[**store_lightning_addresses_get_store_lightning_addresses**](LightningAddressApi.md#store_lightning_addresses_get_store_lightning_addresses) | **GET** /api/v1/stores/{storeId}/lightning-addresses | Get store configured lightning addresses
[**store_lightning_addresses_remove_store_lightning_address**](LightningAddressApi.md#store_lightning_addresses_remove_store_lightning_address) | **DELETE** /api/v1/stores/{storeId}/lightning-addresses/{username} | Remove configured lightning address



## store_lightning_addresses_add_or_update_store_lightning_address

> models::LightningAddressData store_lightning_addresses_add_or_update_store_lightning_address(store_id, username, lightning_address_data)
Add or update store configured lightning address

Add or update store configured lightning address

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |
**username** | **String** | the lightning address username | [required] |
**lightning_address_data** | [**LightningAddressData**](LightningAddressData.md) |  | [required] |

### Return type

[**models::LightningAddressData**](LightningAddressData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_lightning_addresses_get_store_lightning_address

> models::LightningAddressData store_lightning_addresses_get_store_lightning_address(store_id, username)
Get store configured lightning address

Get store configured lightning address

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |
**username** | **String** | The lightning address username | [required] |

### Return type

[**models::LightningAddressData**](LightningAddressData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_lightning_addresses_get_store_lightning_addresses

> Vec<models::LightningAddressData> store_lightning_addresses_get_store_lightning_addresses(store_id)
Get store configured lightning addresses

Get store configured lightning addresses

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |

### Return type

[**Vec<models::LightningAddressData>**](LightningAddressData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_lightning_addresses_remove_store_lightning_address

> store_lightning_addresses_remove_store_lightning_address(store_id, username)
Remove configured lightning address

Remove store configured lightning address

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |
**username** | **String** | The lightning address username | [required] |

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

