# \CrowdfundApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**apps_create_crowdfund_app**](CrowdfundApi.md#apps_create_crowdfund_app) | **POST** /api/v1/stores/{storeId}/apps/crowdfund | Create a new Crowdfund app
[**apps_get_crowdfund_app**](CrowdfundApi.md#apps_get_crowdfund_app) | **GET** /api/v1/apps/crowdfund/{appId} | Get crowdfund app data



## apps_create_crowdfund_app

> models::CrowdfundAppData apps_create_crowdfund_app(store_id, crowdfund_app_request)
Create a new Crowdfund app

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |
**crowdfund_app_request** | [**CrowdfundAppRequest**](CrowdfundAppRequest.md) |  | [required] |

### Return type

[**models::CrowdfundAppData**](CrowdfundAppData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## apps_get_crowdfund_app

> models::CrowdfundAppData apps_get_crowdfund_app(app_id)
Get crowdfund app data

Returns crowdfund app data

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**app_id** | **String** | App ID | [required] |

### Return type

[**models::CrowdfundAppData**](CrowdfundAppData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

