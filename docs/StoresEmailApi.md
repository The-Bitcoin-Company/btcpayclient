# \StoresEmailApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**stores_get_store_email_settings**](StoresEmailApi.md#stores_get_store_email_settings) | **GET** /api/v1/stores/{storeId}/email | Get store email settings
[**stores_send_store_email**](StoresEmailApi.md#stores_send_store_email) | **POST** /api/v1/stores/{storeId}/email/send | Send an email for a store
[**stores_update_store_email_settings**](StoresEmailApi.md#stores_update_store_email_settings) | **PUT** /api/v1/stores/{storeId}/email | Update store email settings



## stores_get_store_email_settings

> models::GetEmailSettings stores_get_store_email_settings(store_id)
Get store email settings

Retrieve the email settings configured for specific store. The password field will be masked if present.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |

### Return type

[**models::GetEmailSettings**](GetEmailSettings.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## stores_send_store_email

> stores_send_store_email(store_id, stores_send_store_email_request)
Send an email for a store

Send an email using the store's SMTP server

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |
**stores_send_store_email_request** | [**StoresSendStoreEmailRequest**](StoresSendStoreEmailRequest.md) |  | [required] |

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## stores_update_store_email_settings

> models::GetEmailSettings stores_update_store_email_settings(store_id, update_email_settings)
Update store email settings

Update a store's email settings

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |
**update_email_settings** | [**UpdateEmailSettings**](UpdateEmailSettings.md) |  | [required] |

### Return type

[**models::GetEmailSettings**](GetEmailSettings.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

