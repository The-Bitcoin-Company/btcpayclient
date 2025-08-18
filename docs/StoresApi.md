# \StoresApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**stores_create_store**](StoresApi.md#stores_create_store) | **POST** /api/v1/stores | Create a new store
[**stores_delete_store**](StoresApi.md#stores_delete_store) | **DELETE** /api/v1/stores/{storeId} | Remove Store
[**stores_delete_store_logo**](StoresApi.md#stores_delete_store_logo) | **DELETE** /api/v1/stores/{storeId}/logo | Deletes the store logo
[**stores_get_store**](StoresApi.md#stores_get_store) | **GET** /api/v1/stores/{storeId} | Get store
[**stores_get_store_roles**](StoresApi.md#stores_get_store_roles) | **GET** /api/v1/stores/{storeId}/roles | Get store's roles
[**stores_get_stores**](StoresApi.md#stores_get_stores) | **GET** /api/v1/stores | Get stores
[**stores_update_store**](StoresApi.md#stores_update_store) | **PUT** /api/v1/stores/{storeId} | Update store
[**stores_upload_store_logo**](StoresApi.md#stores_upload_store_logo) | **POST** /api/v1/stores/{storeId}/logo | Uploads a logo for the store



## stores_create_store

> models::StoreData stores_create_store(store_base_data)
Create a new store

Create a new store (default values can be different if the server settings use a default store template)

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_base_data** | [**StoreBaseData**](StoreBaseData.md) |  | [required] |

### Return type

[**models::StoreData**](StoreData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## stores_delete_store

> stores_delete_store(store_id)
Remove Store

Removes the specified store. If there is another user with access, only your access will be removed.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## stores_delete_store_logo

> stores_delete_store_logo(store_id)
Deletes the store logo

Delete the store's logo

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## stores_get_store

> models::StoreData stores_get_store(store_id)
Get store

View information about the specified store

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |

### Return type

[**models::StoreData**](StoreData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## stores_get_store_roles

> models::RoleData stores_get_store_roles(store_id)
Get store's roles

View information about the specified store's roles

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |

### Return type

[**models::RoleData**](RoleData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## stores_get_stores

> Vec<models::StoreData> stores_get_stores()
Get stores

View information about the available stores

### Parameters

This endpoint does not need any parameter.

### Return type

[**Vec<models::StoreData>**](StoreData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## stores_update_store

> models::StoreData stores_update_store(store_id, store_data)
Update store

Update the specified store (default values can be different if the server settings use a default store template)

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |
**store_data** | [**StoreData**](StoreData.md) |  | [required] |

### Return type

[**models::StoreData**](StoreData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## stores_upload_store_logo

> models::ApplicationUserData stores_upload_store_logo(store_id, file)
Uploads a logo for the store

Uploads a logo for the store

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |
**file** | Option<**std::path::PathBuf**> | The logo |  |

### Return type

[**models::ApplicationUserData**](ApplicationUserData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

