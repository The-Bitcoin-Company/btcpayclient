# \AppsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**app_delete_app_item_image**](AppsApi.md#app_delete_app_item_image) | **DELETE** /api/v1/apps/{appId}/image/{fileId} | Deletes the app item image
[**apps_create_crowdfund_app**](AppsApi.md#apps_create_crowdfund_app) | **POST** /api/v1/stores/{storeId}/apps/crowdfund | Create a new Crowdfund app
[**apps_create_point_of_sale_app**](AppsApi.md#apps_create_point_of_sale_app) | **POST** /api/v1/stores/{storeId}/apps/pos | Create a new Point of Sale app
[**apps_delete_app**](AppsApi.md#apps_delete_app) | **DELETE** /api/v1/apps/{appId} | Delete app
[**apps_get_all_apps**](AppsApi.md#apps_get_all_apps) | **GET** /api/v1/apps | Get basic app data for all apps for all stores for a user
[**apps_get_all_apps_for_store**](AppsApi.md#apps_get_all_apps_for_store) | **GET** /api/v1/stores/{storeId}/apps | Get basic app data for all apps for a store
[**apps_get_app**](AppsApi.md#apps_get_app) | **GET** /api/v1/apps/{appId} | Get basic app data
[**apps_get_app_sales**](AppsApi.md#apps_get_app_sales) | **GET** /api/v1/apps/{appId}/sales | Get app sales statistics
[**apps_get_app_top_items**](AppsApi.md#apps_get_app_top_items) | **GET** /api/v1/apps/{appId}/top-items | Get app top items statistics
[**apps_get_crowdfund_app**](AppsApi.md#apps_get_crowdfund_app) | **GET** /api/v1/apps/crowdfund/{appId} | Get crowdfund app data
[**apps_get_point_of_sale_app**](AppsApi.md#apps_get_point_of_sale_app) | **GET** /api/v1/apps/pos/{appId} | Get Point of Sale app data
[**apps_put_point_of_sale_app**](AppsApi.md#apps_put_point_of_sale_app) | **PUT** /api/v1/apps/pos/{appId} | Update a Point of Sale app
[**apps_upload_app_item_image**](AppsApi.md#apps_upload_app_item_image) | **POST** /api/v1/apps/{appId}/image | Uploads an image for a app item



## app_delete_app_item_image

> app_delete_app_item_image(app_id, file_id)
Deletes the app item image

Deletes the app item image

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**app_id** | **String** | App ID | [required] |
**file_id** | **String** | The file ID | [required] |

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


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


## apps_create_point_of_sale_app

> models::PointOfSaleAppData apps_create_point_of_sale_app(store_id, point_of_sale_app_request)
Create a new Point of Sale app

Point of Sale app allows accepting payments for items in a virtual store

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |
**point_of_sale_app_request** | [**PointOfSaleAppRequest**](PointOfSaleAppRequest.md) |  | [required] |

### Return type

[**models::PointOfSaleAppData**](PointOfSaleAppData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## apps_delete_app

> apps_delete_app(app_id)
Delete app

Deletes apps with specified ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**app_id** | **String** | App ID | [required] |

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## apps_get_all_apps

> Vec<models::AppBaseData> apps_get_all_apps()
Get basic app data for all apps for all stores for a user

Returns basic app data for all apps for all stores

### Parameters

This endpoint does not need any parameter.

### Return type

[**Vec<models::AppBaseData>**](AppBaseData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## apps_get_all_apps_for_store

> Vec<models::AppBaseData> apps_get_all_apps_for_store(store_id)
Get basic app data for all apps for a store

Returns basic app data for all apps for a store

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |

### Return type

[**Vec<models::AppBaseData>**](AppBaseData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## apps_get_app

> models::AppBaseData apps_get_app(app_id)
Get basic app data

Returns basic app data shared between all types of apps

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**app_id** | **String** | App ID | [required] |

### Return type

[**models::AppBaseData**](AppBaseData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## apps_get_app_sales

> models::AppSalesStats apps_get_app_sales(app_id, number_of_days)
Get app sales statistics

Returns sales statistics for the app

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**app_id** | **String** | App ID | [required] |
**number_of_days** | Option<**f64**> | How many of the last days |  |[default to 7]

### Return type

[**models::AppSalesStats**](AppSalesStats.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## apps_get_app_top_items

> Vec<models::AppItemStats> apps_get_app_top_items(app_id, count, offset)
Get app top items statistics

Returns top items statistics for the app

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**app_id** | **String** | App ID | [required] |
**count** | Option<**f64**> | How many of the items |  |[default to 5]
**offset** | Option<**f64**> | Offset for paging |  |[default to 0]

### Return type

[**Vec<models::AppItemStats>**](AppItemStats.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
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


## apps_put_point_of_sale_app

> models::PointOfSaleAppData apps_put_point_of_sale_app(app_id, point_of_sale_app_request)
Update a Point of Sale app

Use this endpoint for updating the properties of a POS app

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**app_id** | **String** | App ID | [required] |
**point_of_sale_app_request** | [**PointOfSaleAppRequest**](PointOfSaleAppRequest.md) |  | [required] |

### Return type

[**models::PointOfSaleAppData**](PointOfSaleAppData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## apps_upload_app_item_image

> models::FileData apps_upload_app_item_image(app_id, file)
Uploads an image for a app item

Uploads an image for a app item

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**app_id** | **String** | App ID | [required] |
**file** | Option<**std::path::PathBuf**> | The image |  |

### Return type

[**models::FileData**](FileData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

