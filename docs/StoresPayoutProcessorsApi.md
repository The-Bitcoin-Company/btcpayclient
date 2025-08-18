# \StoresPayoutProcessorsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**greenfield_store_automated_lightning_payout_processors_controller_get_store_lightning_automated_payout_processors_for_payment_method**](StoresPayoutProcessorsApi.md#greenfield_store_automated_lightning_payout_processors_controller_get_store_lightning_automated_payout_processors_for_payment_method) | **GET** /api/v1/stores/{storeId}/payout-processors/LightningAutomatedPayoutSenderFactory/{payoutMethodId} | Get configured store Lightning automated payout processors
[**greenfield_store_automated_lightning_payout_processors_controller_get_store_lightning_automated_payout_sender_factory**](StoresPayoutProcessorsApi.md#greenfield_store_automated_lightning_payout_processors_controller_get_store_lightning_automated_payout_sender_factory) | **GET** /api/v1/stores/{storeId}/payout-processors/LightningAutomatedPayoutSenderFactory | Get configured store Lightning automated payout processors
[**greenfield_store_automated_lightning_payout_processors_controller_update_store_lightning_automated_payout_processor**](StoresPayoutProcessorsApi.md#greenfield_store_automated_lightning_payout_processors_controller_update_store_lightning_automated_payout_processor) | **PUT** /api/v1/stores/{storeId}/payout-processors/LightningAutomatedPayoutSenderFactory/{payoutMethodId} | Update configured store Lightning automated payout processors
[**greenfield_store_automated_on_chain_payout_processors_controller_get_store_on_chain_automated_payout_processors_for_payment_method**](StoresPayoutProcessorsApi.md#greenfield_store_automated_on_chain_payout_processors_controller_get_store_on_chain_automated_payout_processors_for_payment_method) | **GET** /api/v1/stores/{storeId}/payout-processors/OnChainAutomatedPayoutSenderFactory/{paymentMethodId} | Get configured store onchain automated payout processors
[**greenfield_store_automated_on_chain_payout_processors_controller_get_store_on_chain_automated_transfer_sender_factory**](StoresPayoutProcessorsApi.md#greenfield_store_automated_on_chain_payout_processors_controller_get_store_on_chain_automated_transfer_sender_factory) | **GET** /api/v1/stores/{storeId}/payout-processors/OnChainAutomatedTransferSenderFactory | Get configured store onchain automated payout processors
[**greenfield_store_automated_on_chain_payout_processors_controller_update_store_on_chain_automated_payout_processor_for_payment_method**](StoresPayoutProcessorsApi.md#greenfield_store_automated_on_chain_payout_processors_controller_update_store_on_chain_automated_payout_processor_for_payment_method) | **PUT** /api/v1/stores/{storeId}/payout-processors/OnChainAutomatedPayoutSenderFactory/{paymentMethodId} | Update configured store onchain automated payout processors
[**greenfield_store_automated_on_chain_payout_processors_controller_update_store_on_chain_automated_transfer_sender_factory**](StoresPayoutProcessorsApi.md#greenfield_store_automated_on_chain_payout_processors_controller_update_store_on_chain_automated_transfer_sender_factory) | **PUT** /api/v1/stores/{storeId}/payout-processors/OnChainAutomatedTransferSenderFactory | Update configured store onchain automated payout processors
[**store_payout_processors_get_store_payout_processors**](StoresPayoutProcessorsApi.md#store_payout_processors_get_store_payout_processors) | **GET** /api/v1/stores/{storeId}/payout-processors | Get store configured payout processors
[**store_payout_processors_remove_store_payout_processor**](StoresPayoutProcessorsApi.md#store_payout_processors_remove_store_payout_processor) | **DELETE** /api/v1/stores/{storeId}/payout-processors/{processor}/{paymentMethodId} | Remove store configured payout processor



## greenfield_store_automated_lightning_payout_processors_controller_get_store_lightning_automated_payout_processors_for_payment_method

> Vec<models::LightningAutomatedTransferSettings> greenfield_store_automated_lightning_payout_processors_controller_get_store_lightning_automated_payout_processors_for_payment_method(payout_method_id, store_id)
Get configured store Lightning automated payout processors

Get configured store Lightning automated payout processors

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**payout_method_id** | **String** | The payout method id | [required] |
**store_id** | **String** | The store ID | [required] |

### Return type

[**Vec<models::LightningAutomatedTransferSettings>**](LightningAutomatedTransferSettings.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## greenfield_store_automated_lightning_payout_processors_controller_get_store_lightning_automated_payout_sender_factory

> Vec<models::LightningAutomatedTransferSettings> greenfield_store_automated_lightning_payout_processors_controller_get_store_lightning_automated_payout_sender_factory(store_id)
Get configured store Lightning automated payout processors

Get configured store Lightning automated payout processors

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |

### Return type

[**Vec<models::LightningAutomatedTransferSettings>**](LightningAutomatedTransferSettings.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## greenfield_store_automated_lightning_payout_processors_controller_update_store_lightning_automated_payout_processor

> models::LightningAutomatedTransferSettings greenfield_store_automated_lightning_payout_processors_controller_update_store_lightning_automated_payout_processor(payout_method_id, store_id, update_lightning_automated_transfer_settings)
Update configured store Lightning automated payout processors

Update configured store Lightning automated payout processors

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**payout_method_id** | **String** | The payout method id | [required] |
**store_id** | **String** | The store ID | [required] |
**update_lightning_automated_transfer_settings** | [**UpdateLightningAutomatedTransferSettings**](UpdateLightningAutomatedTransferSettings.md) |  | [required] |

### Return type

[**models::LightningAutomatedTransferSettings**](LightningAutomatedTransferSettings.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## greenfield_store_automated_on_chain_payout_processors_controller_get_store_on_chain_automated_payout_processors_for_payment_method

> Vec<models::OnChainAutomatedTransferSettings> greenfield_store_automated_on_chain_payout_processors_controller_get_store_on_chain_automated_payout_processors_for_payment_method(payment_method_id, store_id)
Get configured store onchain automated payout processors

Get configured store onchain automated payout processors

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**payment_method_id** | **String** | The payment method id of the payment method to update | [required] |
**store_id** | **String** | The store ID | [required] |

### Return type

[**Vec<models::OnChainAutomatedTransferSettings>**](OnChainAutomatedTransferSettings.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## greenfield_store_automated_on_chain_payout_processors_controller_get_store_on_chain_automated_transfer_sender_factory

> Vec<models::OnChainAutomatedTransferSettings> greenfield_store_automated_on_chain_payout_processors_controller_get_store_on_chain_automated_transfer_sender_factory(store_id)
Get configured store onchain automated payout processors

Get configured store onchain automated payout processors

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |

### Return type

[**Vec<models::OnChainAutomatedTransferSettings>**](OnChainAutomatedTransferSettings.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## greenfield_store_automated_on_chain_payout_processors_controller_update_store_on_chain_automated_payout_processor_for_payment_method

> models::OnChainAutomatedTransferSettings greenfield_store_automated_on_chain_payout_processors_controller_update_store_on_chain_automated_payout_processor_for_payment_method(payment_method_id, store_id, update_on_chain_automated_transfer_settings)
Update configured store onchain automated payout processors

Update configured store onchain automated payout processors

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**payment_method_id** | **String** | The payment method id of the payment method to update | [required] |
**store_id** | **String** | The store ID | [required] |
**update_on_chain_automated_transfer_settings** | [**UpdateOnChainAutomatedTransferSettings**](UpdateOnChainAutomatedTransferSettings.md) |  | [required] |

### Return type

[**models::OnChainAutomatedTransferSettings**](OnChainAutomatedTransferSettings.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## greenfield_store_automated_on_chain_payout_processors_controller_update_store_on_chain_automated_transfer_sender_factory

> models::OnChainAutomatedTransferSettings greenfield_store_automated_on_chain_payout_processors_controller_update_store_on_chain_automated_transfer_sender_factory(store_id, update_on_chain_automated_transfer_settings)
Update configured store onchain automated payout processors

Update configured store onchain automated payout processors

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |
**update_on_chain_automated_transfer_settings** | [**UpdateOnChainAutomatedTransferSettings**](UpdateOnChainAutomatedTransferSettings.md) |  | [required] |

### Return type

[**models::OnChainAutomatedTransferSettings**](OnChainAutomatedTransferSettings.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_payout_processors_get_store_payout_processors

> Vec<models::PayoutProcessorData> store_payout_processors_get_store_payout_processors(store_id)
Get store configured payout processors

Get store configured payout processors

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |

### Return type

[**Vec<models::PayoutProcessorData>**](PayoutProcessorData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_payout_processors_remove_store_payout_processor

> store_payout_processors_remove_store_payout_processor(payment_method_id, store_id, processor)
Remove store configured payout processor

Remove store configured payout processor

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**payment_method_id** | **String** | The payment method id of the payment method to update | [required] |
**store_id** | **String** | The store ID | [required] |
**processor** | **String** | The processor | [required] |

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

