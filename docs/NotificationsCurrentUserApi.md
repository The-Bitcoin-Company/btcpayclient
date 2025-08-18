# \NotificationsCurrentUserApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**notifications_delete_notification**](NotificationsCurrentUserApi.md#notifications_delete_notification) | **DELETE** /api/v1/users/me/notifications/{id} | Remove Notification
[**notifications_get_notification**](NotificationsCurrentUserApi.md#notifications_get_notification) | **GET** /api/v1/users/me/notifications/{id} | Get notification
[**notifications_get_notification_settings**](NotificationsCurrentUserApi.md#notifications_get_notification_settings) | **GET** /api/v1/users/me/notification-settings | Get notification settings
[**notifications_get_notifications**](NotificationsCurrentUserApi.md#notifications_get_notifications) | **GET** /api/v1/users/me/notifications | Get notifications
[**notifications_update_notification**](NotificationsCurrentUserApi.md#notifications_update_notification) | **PUT** /api/v1/users/me/notifications/{id} | Update notification
[**notifications_update_notification_settings**](NotificationsCurrentUserApi.md#notifications_update_notification_settings) | **PUT** /api/v1/users/me/notification-settings | Update notification settings



## notifications_delete_notification

> notifications_delete_notification(id)
Remove Notification

Removes the specified notification.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | The notification to remove | [required] |

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## notifications_get_notification

> models::NotificationData notifications_get_notification(id)
Get notification

View information about the specified notification

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | The notification to fetch | [required] |

### Return type

[**models::NotificationData**](NotificationData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## notifications_get_notification_settings

> models::NotificationSettingsData notifications_get_notification_settings()
Get notification settings

View information about your notification settings

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::NotificationSettingsData**](NotificationSettingsData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## notifications_get_notifications

> models::NotificationData notifications_get_notifications(store_id, take, skip, seen)
Get notifications

View current user's notifications

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | Option<[**Vec<String>**](String.md)> | Array of store ids to fetch the notifications for |  |
**take** | Option<**f64**> | Number of records returned in response |  |
**skip** | Option<**f64**> | Number of records to skip |  |
**seen** | Option<**String**> | filter by seen notifications |  |

### Return type

[**models::NotificationData**](NotificationData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## notifications_update_notification

> models::NotificationData notifications_update_notification(id, update_notification)
Update notification

Updates the notification

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | The notification to update | [required] |
**update_notification** | [**UpdateNotification**](UpdateNotification.md) |  | [required] |

### Return type

[**models::NotificationData**](NotificationData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## notifications_update_notification_settings

> models::NotificationSettingsData notifications_update_notification_settings(update_notification_settings_request)
Update notification settings

Updates the current user's notification settings

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**update_notification_settings_request** | [**UpdateNotificationSettingsRequest**](UpdateNotificationSettingsRequest.md) |  | [required] |

### Return type

[**models::NotificationSettingsData**](NotificationSettingsData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

