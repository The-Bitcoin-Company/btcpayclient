# \PullPaymentsPublicApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**pull_payments_create_payout**](PullPaymentsPublicApi.md#pull_payments_create_payout) | **POST** /api/v1/pull-payments/{pullPaymentId}/payouts | Create Payout
[**pull_payments_get_payout**](PullPaymentsPublicApi.md#pull_payments_get_payout) | **GET** /api/v1/pull-payments/{pullPaymentId}/payouts/{payoutId} | Get Payout
[**pull_payments_get_payouts**](PullPaymentsPublicApi.md#pull_payments_get_payouts) | **GET** /api/v1/pull-payments/{pullPaymentId}/payouts | Get Payouts
[**pull_payments_get_pull_payment**](PullPaymentsPublicApi.md#pull_payments_get_pull_payment) | **GET** /api/v1/pull-payments/{pullPaymentId} | Get Pull Payment
[**pull_payments_get_pull_payment_lnurl**](PullPaymentsPublicApi.md#pull_payments_get_pull_payment_lnurl) | **GET** /api/v1/pull-payments/{pullPaymentId}/lnurl | Get Pull Payment LNURL details
[**pull_payments_link_boltcard**](PullPaymentsPublicApi.md#pull_payments_link_boltcard) | **POST** /api/v1/pull-payments/{pullPaymentId}/boltcards | Link a boltcard to a pull payment



## pull_payments_create_payout

> models::PayoutData pull_payments_create_payout(pull_payment_id, create_payout_request)
Create Payout

Create a new payout

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pull_payment_id** | **String** | The ID of the pull payment | [required] |
**create_payout_request** | [**CreatePayoutRequest**](CreatePayoutRequest.md) |  | [required] |

### Return type

[**models::PayoutData**](PayoutData.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## pull_payments_get_payout

> models::PayoutData pull_payments_get_payout(pull_payment_id, payout_id)
Get Payout

Get payout

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pull_payment_id** | **String** | The ID of the pull payment | [required] |
**payout_id** | **String** | The ID of the pull payment payout | [required] |

### Return type

[**models::PayoutData**](PayoutData.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## pull_payments_get_payouts

> Vec<models::PayoutData> pull_payments_get_payouts(pull_payment_id, include_cancelled)
Get Payouts

Get payouts

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pull_payment_id** | **String** | The ID of the pull payment | [required] |
**include_cancelled** | Option<**bool**> | Whether this should list cancelled payouts |  |[default to false]

### Return type

[**Vec<models::PayoutData>**](PayoutData.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## pull_payments_get_pull_payment

> models::PullPaymentData pull_payments_get_pull_payment(pull_payment_id)
Get Pull Payment

Get a pull payment

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pull_payment_id** | **String** | The ID of the pull payment | [required] |

### Return type

[**models::PullPaymentData**](PullPaymentData.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## pull_payments_get_pull_payment_lnurl

> models::LnurlData pull_payments_get_pull_payment_lnurl(pull_payment_id)
Get Pull Payment LNURL details

Get Pull Payment LNURL details

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pull_payment_id** | **String** | The ID of the pull payment | [required] |

### Return type

[**models::LnurlData**](LNURLData.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## pull_payments_link_boltcard

> models::PullPaymentsLinkBoltcard200Response pull_payments_link_boltcard(pull_payment_id, pull_payments_link_boltcard_request)
Link a boltcard to a pull payment

Linking a boltcard to a pull payment will allow you to pay via NFC with it, the money will be sent from the pull payment. The boltcard keys are generated using [Deterministic Boltcard Key Generation](https://github.com/boltcard/boltcard/blob/main/docs/DETERMINISTIC.md).

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pull_payment_id** | **String** | The ID of the pull payment | [required] |
**pull_payments_link_boltcard_request** | Option<[**PullPaymentsLinkBoltcardRequest**](PullPaymentsLinkBoltcardRequest.md)> |  |  |

### Return type

[**models::PullPaymentsLinkBoltcard200Response**](PullPayments_LinkBoltcard_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

