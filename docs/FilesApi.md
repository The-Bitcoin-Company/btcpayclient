# \FilesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**files_delete_file**](FilesApi.md#files_delete_file) | **DELETE** /api/v1/files/{fileId} | Delete file
[**files_get_file**](FilesApi.md#files_get_file) | **GET** /api/v1/files/{fileId} | Get file
[**files_get_files**](FilesApi.md#files_get_files) | **GET** /api/v1/files | Get all files
[**files_upload_file**](FilesApi.md#files_upload_file) | **POST** /api/v1/files | Uploads a file



## files_delete_file

> files_delete_file(file_id)
Delete file

Deletes the file

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**file_id** | **String** | The file to delete | [required] |

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## files_get_file

> models::FileData files_get_file(file_id)
Get file

View information about the specified file

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**file_id** | **String** | The file information to fetch | [required] |

### Return type

[**models::FileData**](FileData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## files_get_files

> Vec<models::FileData> files_get_files()
Get all files

Load all files that exist.

### Parameters

This endpoint does not need any parameter.

### Return type

[**Vec<models::FileData>**](FileData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## files_upload_file

> models::FileData files_upload_file(file)
Uploads a file

Uploads a file

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**file** | Option<**std::path::PathBuf**> | The profile picture |  |

### Return type

[**models::FileData**](FileData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

