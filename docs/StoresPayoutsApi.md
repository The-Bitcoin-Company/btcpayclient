# \StoresPayoutsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_store_payout**](StoresPayoutsApi.md#get_store_payout) | **GET** /api/v1/stores/{storeId}/payouts/{payoutId} | Get Payout
[**payouts_create_payout_through_store**](StoresPayoutsApi.md#payouts_create_payout_through_store) | **POST** /api/v1/stores/{storeId}/payouts | Create Payout
[**pull_payments_approve_payout**](StoresPayoutsApi.md#pull_payments_approve_payout) | **POST** /api/v1/stores/{storeId}/payouts/{payoutId} | Approve Payout
[**pull_payments_cancel_payout**](StoresPayoutsApi.md#pull_payments_cancel_payout) | **DELETE** /api/v1/stores/{storeId}/payouts/{payoutId} | Cancel Payout
[**pull_payments_get_store_payouts**](StoresPayoutsApi.md#pull_payments_get_store_payouts) | **GET** /api/v1/stores/{storeId}/payouts | Get Store Payouts
[**pull_payments_mark_payout**](StoresPayoutsApi.md#pull_payments_mark_payout) | **POST** /api/v1/stores/{storeId}/payouts/{payoutId}/mark | Mark Payout
[**pull_payments_mark_payout_paid**](StoresPayoutsApi.md#pull_payments_mark_payout_paid) | **POST** /api/v1/stores/{storeId}/payouts/{payoutId}/mark-paid | Mark Payout as Paid



## get_store_payout

> models::PayoutData get_store_payout(store_id, payout_id)
Get Payout

Get payout

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |
**payout_id** | **String** | The ID of the payout | [required] |

### Return type

[**models::PayoutData**](PayoutData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## payouts_create_payout_through_store

> models::PayoutData payouts_create_payout_through_store(store_id, create_payout_through_store_request)
Create Payout

Create a new payout

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |
**create_payout_through_store_request** | [**CreatePayoutThroughStoreRequest**](CreatePayoutThroughStoreRequest.md) |  | [required] |

### Return type

[**models::PayoutData**](PayoutData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## pull_payments_approve_payout

> models::PayoutData pull_payments_approve_payout(store_id, payout_id, pull_payments_approve_payout_request)
Approve Payout

Approve a payout

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |
**payout_id** | **String** | The ID of the payout | [required] |
**pull_payments_approve_payout_request** | Option<[**PullPaymentsApprovePayoutRequest**](PullPaymentsApprovePayoutRequest.md)> |  |  |

### Return type

[**models::PayoutData**](PayoutData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## pull_payments_cancel_payout

> pull_payments_cancel_payout(store_id, payout_id)
Cancel Payout

Cancel the payout

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |
**payout_id** | **String** | The ID of the payout | [required] |

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## pull_payments_get_store_payouts

> Vec<models::PayoutData> pull_payments_get_store_payouts(store_id, include_cancelled)
Get Store Payouts

Get payouts

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |
**include_cancelled** | Option<**bool**> | Whether this should list cancelled payouts |  |[default to false]

### Return type

[**Vec<models::PayoutData>**](PayoutData.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## pull_payments_mark_payout

> pull_payments_mark_payout(store_id, payout_id, pull_payments_mark_payout_request)
Mark Payout

Mark a payout with a state

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |
**payout_id** | **String** | The ID of the payout | [required] |
**pull_payments_mark_payout_request** | Option<[**PullPaymentsMarkPayoutRequest**](PullPaymentsMarkPayoutRequest.md)> |  |  |

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## pull_payments_mark_payout_paid

> pull_payments_mark_payout_paid(store_id, payout_id)
Mark Payout as Paid

Mark a payout as paid

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |
**payout_id** | **String** | The ID of the payout | [required] |

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

