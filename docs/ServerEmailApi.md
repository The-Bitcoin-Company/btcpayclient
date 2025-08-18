# \ServerEmailApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**server_email_get_settings**](ServerEmailApi.md#server_email_get_settings) | **GET** /api/v1/server/email | Get server email settings
[**server_email_update_settings**](ServerEmailApi.md#server_email_update_settings) | **PUT** /api/v1/server/email | Update server email settings



## server_email_get_settings

> models::GetServerEmailSettings server_email_get_settings()
Get server email settings

Retrieve the email settings configured for the server. The password field will be masked if present.

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::GetServerEmailSettings**](GetServerEmailSettings.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## server_email_update_settings

> models::GetServerEmailSettings server_email_update_settings(update_server_email_settings)
Update server email settings

Update server's email settings.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**update_server_email_settings** | [**UpdateServerEmailSettings**](UpdateServerEmailSettings.md) |  | [required] |

### Return type

[**models::GetServerEmailSettings**](GetServerEmailSettings.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

