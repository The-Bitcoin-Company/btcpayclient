# \UsersApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**users_create_user**](UsersApi.md#users_create_user) | **POST** /api/v1/users | Create user
[**users_delete_current_user**](UsersApi.md#users_delete_current_user) | **DELETE** /api/v1/users/me | Deletes user profile
[**users_delete_current_user_profile_picture**](UsersApi.md#users_delete_current_user_profile_picture) | **DELETE** /api/v1/users/me/picture | Deletes user profile picture
[**users_delete_user**](UsersApi.md#users_delete_user) | **DELETE** /api/v1/users/{idOrEmail} | Delete user
[**users_get_current_user**](UsersApi.md#users_get_current_user) | **GET** /api/v1/users/me | Get current user information
[**users_get_user**](UsersApi.md#users_get_user) | **GET** /api/v1/users/{idOrEmail} | Get user by ID or Email
[**users_get_users**](UsersApi.md#users_get_users) | **GET** /api/v1/users | Get all users
[**users_toggle_user_approval**](UsersApi.md#users_toggle_user_approval) | **POST** /api/v1/users/{idOrEmail}/approve | Toggle user approval
[**users_toggle_user_lock**](UsersApi.md#users_toggle_user_lock) | **POST** /api/v1/users/{idOrEmail}/lock | Toggle user lock out
[**users_update_current_user**](UsersApi.md#users_update_current_user) | **PUT** /api/v1/users/me | Update current user information
[**users_upload_current_user_profile_picture**](UsersApi.md#users_upload_current_user_profile_picture) | **POST** /api/v1/users/me/picture | Uploads a profile picture for the current user



## users_create_user

> models::ApplicationUserData users_create_user(users_create_user_request)
Create user

Create a new user.  This operation can be called without authentication in any of this cases: * There is not any administrator yet on the server, * User registrations are not disabled in the server's policies.  If the first administrator is created by this call, user registrations are automatically disabled.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**users_create_user_request** | [**UsersCreateUserRequest**](UsersCreateUserRequest.md) |  | [required] |

### Return type

[**models::ApplicationUserData**](ApplicationUserData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## users_delete_current_user

> users_delete_current_user()
Deletes user profile

Deletes user profile and associated user data for user making the request

### Parameters

This endpoint does not need any parameter.

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## users_delete_current_user_profile_picture

> users_delete_current_user_profile_picture()
Deletes user profile picture

Deletes the user profile picture

### Parameters

This endpoint does not need any parameter.

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## users_delete_user

> users_delete_user(id_or_email)
Delete user

Delete a user.  Must be an admin to perform this operation.  Attempting to delete the only admin user will not succeed.  All data associated with the user will be deleted as well if the operation succeeds.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id_or_email** | **String** | The user's id or email | [required] |

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## users_get_current_user

> models::ApplicationUserData users_get_current_user()
Get current user information

View information about the current user

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::ApplicationUserData**](ApplicationUserData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## users_get_user

> models::ApplicationUserData users_get_user(id_or_email)
Get user by ID or Email

Get 1 user by ID or Email.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id_or_email** | **String** | The user's id or email | [required] |

### Return type

[**models::ApplicationUserData**](ApplicationUserData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## users_get_users

> users_get_users()
Get all users

Load all users that exist.

### Parameters

This endpoint does not need any parameter.

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## users_toggle_user_approval

> users_toggle_user_approval(id_or_email, approve_user_request)
Toggle user approval

Approve or unapprove a user.  Must be an admin to perform this operation.  Attempting to (un)approve a user for which this requirement does not exist will not succeed.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id_or_email** | **String** | The user's id or email | [required] |
**approve_user_request** | Option<[**ApproveUserRequest**](ApproveUserRequest.md)> |  |  |

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## users_toggle_user_lock

> users_toggle_user_lock(id_or_email, lock_user_request)
Toggle user lock out

Lock or unlock a user.  Must be an admin to perform this operation.  Attempting to lock the only admin user will not succeed.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id_or_email** | **String** | The user's id or email | [required] |
**lock_user_request** | Option<[**LockUserRequest**](LockUserRequest.md)> |  |  |

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## users_update_current_user

> models::ApplicationUserData users_update_current_user(users_update_current_user_request)
Update current user information

Update the current user

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**users_update_current_user_request** | [**UsersUpdateCurrentUserRequest**](UsersUpdateCurrentUserRequest.md) |  | [required] |

### Return type

[**models::ApplicationUserData**](ApplicationUserData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## users_upload_current_user_profile_picture

> models::ApplicationUserData users_upload_current_user_profile_picture(file)
Uploads a profile picture for the current user

Uploads a profile picture for the current user

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**file** | Option<**std::path::PathBuf**> | The profile picture |  |

### Return type

[**models::ApplicationUserData**](ApplicationUserData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

