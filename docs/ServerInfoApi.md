# \ServerInfoApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**server_get_store_roles**](ServerInfoApi.md#server_get_store_roles) | **GET** /api/v1/server/roles | Get store's roles
[**server_info_get_server_info**](ServerInfoApi.md#server_info_get_server_info) | **GET** /api/v1/server/info | Get server info



## server_get_store_roles

> models::RoleData server_get_store_roles()
Get store's roles

View information about the store's roles at the server's scope

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::RoleData**](RoleData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## server_info_get_server_info

> models::ApplicationServerInfoData server_info_get_server_info()
Get server info

Information about the server, chains and sync states

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::ApplicationServerInfoData**](ApplicationServerInfoData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

