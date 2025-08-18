# \PointOfSaleApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**apps_get_point_of_sale_app**](PointOfSaleApi.md#apps_get_point_of_sale_app) | **GET** /api/v1/apps/pos/{appId} | Get Point of Sale app data



## apps_get_point_of_sale_app

> models::PointOfSaleAppData apps_get_point_of_sale_app(app_id)
Get Point of Sale app data

Returns POS app data

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**app_id** | **String** | App ID | [required] |

### Return type

[**models::PointOfSaleAppData**](PointOfSaleAppData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

