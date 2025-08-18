# \StoresUsersApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**stores_add_store_user**](StoresUsersApi.md#stores_add_store_user) | **POST** /api/v1/stores/{storeId}/users | Add a store user
[**stores_get_store_users**](StoresUsersApi.md#stores_get_store_users) | **GET** /api/v1/stores/{storeId}/users | Get store users
[**stores_remove_store_user**](StoresUsersApi.md#stores_remove_store_user) | **DELETE** /api/v1/stores/{storeId}/users/{idOrEmail} | Remove Store User
[**stores_update_store_user**](StoresUsersApi.md#stores_update_store_user) | **PUT** /api/v1/stores/{storeId}/users/{idOrEmail} | Updates a store user



## stores_add_store_user

> stores_add_store_user(store_id, store_user_data)
Add a store user

Add a store user

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |
**store_user_data** | [**StoreUserData**](StoreUserData.md) |  | [required] |

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## stores_get_store_users

> Vec<models::StoreUserData> stores_get_store_users(store_id)
Get store users

View users of the specified store

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |

### Return type

[**Vec<models::StoreUserData>**](StoreUserData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## stores_remove_store_user

> stores_remove_store_user(store_id, id_or_email)
Remove Store User

Removes the specified store user. If there is no other owner, this endpoint will fail.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |
**id_or_email** | **String** | The user's id or email | [required] |

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## stores_update_store_user

> stores_update_store_user(store_id, id_or_email, store_user_data)
Updates a store user

Updates a store user

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |
**id_or_email** | **String** | The user's id or email | [required] |
**store_user_data** | [**StoreUserData**](StoreUserData.md) |  | [required] |

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

