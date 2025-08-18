# \WebhooksApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**webhooks_create_webhook**](WebhooksApi.md#webhooks_create_webhook) | **POST** /api/v1/stores/{storeId}/webhooks | Create a new webhook
[**webhooks_delete_webhook**](WebhooksApi.md#webhooks_delete_webhook) | **DELETE** /api/v1/stores/{storeId}/webhooks/{webhookId} | Delete a webhook
[**webhooks_get_webhook**](WebhooksApi.md#webhooks_get_webhook) | **GET** /api/v1/stores/{storeId}/webhooks/{webhookId} | Get a webhook of a store
[**webhooks_get_webhook_deliveries**](WebhooksApi.md#webhooks_get_webhook_deliveries) | **GET** /api/v1/stores/{storeId}/webhooks/{webhookId}/deliveries | Get latest deliveries
[**webhooks_get_webhook_delivery**](WebhooksApi.md#webhooks_get_webhook_delivery) | **GET** /api/v1/stores/{storeId}/webhooks/{webhookId}/deliveries/{deliveryId} | Get a webhook delivery
[**webhooks_get_webhook_delivery_requests**](WebhooksApi.md#webhooks_get_webhook_delivery_requests) | **GET** /api/v1/stores/{storeId}/webhooks/{webhookId}/deliveries/{deliveryId}/request | Get the delivery's request
[**webhooks_get_webhooks**](WebhooksApi.md#webhooks_get_webhooks) | **GET** /api/v1/stores/{storeId}/webhooks | Get webhooks of a store
[**webhooks_redeliver_webhook_delivery**](WebhooksApi.md#webhooks_redeliver_webhook_delivery) | **POST** /api/v1/stores/{storeId}/webhooks/{webhookId}/deliveries/{deliveryId}/redeliver | Redeliver the delivery
[**webhooks_update_webhook**](WebhooksApi.md#webhooks_update_webhook) | **PUT** /api/v1/stores/{storeId}/webhooks/{webhookId} | Update a webhook



## webhooks_create_webhook

> models::WebhookDataCreateResult webhooks_create_webhook(store_id, webhook_data_create)
Create a new webhook

Create a new webhook

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |
**webhook_data_create** | [**WebhookDataCreate**](WebhookDataCreate.md) |  | [required] |

### Return type

[**models::WebhookDataCreateResult**](WebhookDataCreateResult.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## webhooks_delete_webhook

> webhooks_delete_webhook(store_id, webhook_id)
Delete a webhook

Delete a webhook

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |
**webhook_id** | **String** | The webhook id | [required] |

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## webhooks_get_webhook

> models::WebhookData webhooks_get_webhook(store_id, webhook_id)
Get a webhook of a store

View webhook of a store

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |
**webhook_id** | **String** | The webhook id | [required] |

### Return type

[**models::WebhookData**](WebhookData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## webhooks_get_webhook_deliveries

> Vec<models::WebhookDeliveryData> webhooks_get_webhook_deliveries(store_id, webhook_id, count)
Get latest deliveries

List the latest deliveries to the webhook, ordered from the most recent

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |
**webhook_id** | **String** | The webhook id | [required] |
**count** | Option<**String**> | The number of latest deliveries to fetch |  |

### Return type

[**Vec<models::WebhookDeliveryData>**](WebhookDeliveryData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## webhooks_get_webhook_delivery

> models::WebhookDeliveryData webhooks_get_webhook_delivery(delivery_id, store_id, webhook_id)
Get a webhook delivery

Information about a webhook delivery

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**delivery_id** | **String** | The id of the delivery | [required] |
**store_id** | **String** | The store ID | [required] |
**webhook_id** | **String** | The webhook id | [required] |

### Return type

[**models::WebhookDeliveryData**](WebhookDeliveryData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## webhooks_get_webhook_delivery_requests

> std::collections::HashMap<String, serde_json::Value> webhooks_get_webhook_delivery_requests(delivery_id, store_id, webhook_id)
Get the delivery's request

The delivery's JSON request sent to the endpoint

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**delivery_id** | **String** | The id of the delivery | [required] |
**store_id** | **String** | The store ID | [required] |
**webhook_id** | **String** | The webhook id | [required] |

### Return type

[**std::collections::HashMap<String, serde_json::Value>**](serde_json::Value.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## webhooks_get_webhooks

> Vec<models::WebhookData> webhooks_get_webhooks(store_id)
Get webhooks of a store

View webhooks of a store

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |

### Return type

[**Vec<models::WebhookData>**](WebhookData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## webhooks_redeliver_webhook_delivery

> String webhooks_redeliver_webhook_delivery(delivery_id, store_id, webhook_id)
Redeliver the delivery

Redeliver the delivery

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**delivery_id** | **String** | The id of the delivery | [required] |
**store_id** | **String** | The store ID | [required] |
**webhook_id** | **String** | The webhook id | [required] |

### Return type

**String**

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## webhooks_update_webhook

> models::WebhookData webhooks_update_webhook(store_id, webhook_id, webhook_data_update)
Update a webhook

Update a webhook

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |
**webhook_id** | **String** | The webhook id | [required] |
**webhook_data_update** | [**WebhookDataUpdate**](WebhookDataUpdate.md) |  | [required] |

### Return type

[**models::WebhookData**](WebhookData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

