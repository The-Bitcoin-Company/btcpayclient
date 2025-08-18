# \ApiKeysApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**api_keys_create_api_key**](ApiKeysApi.md#api_keys_create_api_key) | **POST** /api/v1/api-keys | Create a new API Key
[**api_keys_create_user_api_key**](ApiKeysApi.md#api_keys_create_user_api_key) | **POST** /api/v1/users/{idOrEmail}/api-keys | Create a new API Key for a user
[**api_keys_delete_api_key**](ApiKeysApi.md#api_keys_delete_api_key) | **DELETE** /api/v1/api-keys/{apikey} | Revoke an API Key
[**api_keys_delete_current_api_key**](ApiKeysApi.md#api_keys_delete_current_api_key) | **DELETE** /api/v1/api-keys/current | Revoke the current API Key
[**api_keys_delete_user_api_key**](ApiKeysApi.md#api_keys_delete_user_api_key) | **DELETE** /api/v1/users/{idOrEmail}/api-keys/{apikey} | Revoke an API Key of target user
[**api_keys_get_current_api_key**](ApiKeysApi.md#api_keys_get_current_api_key) | **GET** /api/v1/api-keys/current | Get the current API Key information



## api_keys_create_api_key

> models::ApiKeyData api_keys_create_api_key(api_keys_create_api_key_request)
Create a new API Key

Create a new API Key

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_keys_create_api_key_request** | Option<[**ApiKeysCreateApiKeyRequest**](ApiKeysCreateApiKeyRequest.md)> |  |  |

### Return type

[**models::ApiKeyData**](ApiKeyData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## api_keys_create_user_api_key

> models::ApiKeyData api_keys_create_user_api_key(id_or_email, api_keys_create_api_key_request)
Create a new API Key for a user

Create a new API Key for a user

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id_or_email** | **String** | The user's id or email | [required] |
**api_keys_create_api_key_request** | Option<[**ApiKeysCreateApiKeyRequest**](ApiKeysCreateApiKeyRequest.md)> |  |  |

### Return type

[**models::ApiKeyData**](ApiKeyData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## api_keys_delete_api_key

> api_keys_delete_api_key(apikey)
Revoke an API Key

Revoke the current API key so that it cannot be used anymore

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**apikey** | **String** | The API Key to revoke | [required] |

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## api_keys_delete_current_api_key

> models::ApiKeyData api_keys_delete_current_api_key()
Revoke the current API Key

Revoke the current API key so that it cannot be used anymore

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::ApiKeyData**](ApiKeyData.md)

### Authorization

[API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## api_keys_delete_user_api_key

> api_keys_delete_user_api_key(id_or_email, apikey)
Revoke an API Key of target user

Revoke the API key of a target user so that it cannot be used anymore

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id_or_email** | **String** | The user's id or email | [required] |
**apikey** | **String** | The API Key to revoke | [required] |

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## api_keys_get_current_api_key

> models::ApiKeyData api_keys_get_current_api_key()
Get the current API Key information

View information about the current API key

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::ApiKeyData**](ApiKeyData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

