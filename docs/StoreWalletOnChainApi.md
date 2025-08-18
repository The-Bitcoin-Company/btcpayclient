# \StoreWalletOnChainApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**store_on_chain_payment_methods_generate_on_chain_wallet**](StoreWalletOnChainApi.md#store_on_chain_payment_methods_generate_on_chain_wallet) | **POST** /api/v1/stores/{storeId}/payment-methods/{paymentMethodId}/wallet/generate | Generate store on-chain wallet
[**store_on_chain_payment_methods_get_on_chain_payment_method_preview**](StoreWalletOnChainApi.md#store_on_chain_payment_methods_get_on_chain_payment_method_preview) | **GET** /api/v1/stores/{storeId}/payment-methods/{paymentMethodId}/wallet/preview | Preview store on-chain payment method addresses
[**store_on_chain_payment_methods_poston_chain_payment_method_preview**](StoreWalletOnChainApi.md#store_on_chain_payment_methods_poston_chain_payment_method_preview) | **POST** /api/v1/stores/{storeId}/payment-methods/{paymentMethodId}/wallet/preview | Preview proposed store on-chain payment method addresses
[**store_on_chain_wallets_add_or_update_on_chain_wallet_link**](StoreWalletOnChainApi.md#store_on_chain_wallets_add_or_update_on_chain_wallet_link) | **POST** /api/v1/stores/{storeId}/payment-methods/{paymentMethodId}/wallet/objects/{objectType}/{objectId}/links | Add/Update store on-chain wallet object link
[**store_on_chain_wallets_add_or_update_on_chain_wallet_objects**](StoreWalletOnChainApi.md#store_on_chain_wallets_add_or_update_on_chain_wallet_objects) | **POST** /api/v1/stores/{storeId}/payment-methods/{paymentMethodId}/wallet/objects | Add/Update store on-chain wallet objects
[**store_on_chain_wallets_create_on_chain_transaction**](StoreWalletOnChainApi.md#store_on_chain_wallets_create_on_chain_transaction) | **POST** /api/v1/stores/{storeId}/payment-methods/{paymentMethodId}/wallet/transactions | Create store on-chain wallet transaction
[**store_on_chain_wallets_get_on_chain_fee_rate**](StoreWalletOnChainApi.md#store_on_chain_wallets_get_on_chain_fee_rate) | **GET** /api/v1/stores/{storeId}/payment-methods/{paymentMethodId}/wallet/feerate | Get store on-chain wallet fee rate
[**store_on_chain_wallets_get_on_chain_wallet_object**](StoreWalletOnChainApi.md#store_on_chain_wallets_get_on_chain_wallet_object) | **GET** /api/v1/stores/{storeId}/payment-methods/{paymentMethodId}/wallet/objects/{objectType}/{objectId} | Get store on-chain wallet object
[**store_on_chain_wallets_get_on_chain_wallet_objects**](StoreWalletOnChainApi.md#store_on_chain_wallets_get_on_chain_wallet_objects) | **GET** /api/v1/stores/{storeId}/payment-methods/{paymentMethodId}/wallet/objects | Get store on-chain wallet objects
[**store_on_chain_wallets_get_on_chain_wallet_receive_address**](StoreWalletOnChainApi.md#store_on_chain_wallets_get_on_chain_wallet_receive_address) | **GET** /api/v1/stores/{storeId}/payment-methods/{paymentMethodId}/wallet/address | Get store on-chain wallet address
[**store_on_chain_wallets_get_on_chain_wallet_transaction**](StoreWalletOnChainApi.md#store_on_chain_wallets_get_on_chain_wallet_transaction) | **GET** /api/v1/stores/{storeId}/payment-methods/{paymentMethodId}/wallet/transactions/{transactionId} | Get store on-chain wallet transaction
[**store_on_chain_wallets_get_on_chain_wallet_utxos**](StoreWalletOnChainApi.md#store_on_chain_wallets_get_on_chain_wallet_utxos) | **GET** /api/v1/stores/{storeId}/payment-methods/{paymentMethodId}/wallet/utxos | Get store on-chain wallet UTXOS
[**store_on_chain_wallets_patch_on_chain_wallet_transaction**](StoreWalletOnChainApi.md#store_on_chain_wallets_patch_on_chain_wallet_transaction) | **PATCH** /api/v1/stores/{storeId}/payment-methods/{paymentMethodId}/wallet/transactions/{transactionId} | Patch store on-chain wallet transaction info
[**store_on_chain_wallets_remove_on_chain_wallet_link**](StoreWalletOnChainApi.md#store_on_chain_wallets_remove_on_chain_wallet_link) | **DELETE** /api/v1/stores/{storeId}/payment-methods/{paymentMethodId}/wallet/objects/{objectType}/{objectId}/links/{linkType}/{linkId} | Remove store on-chain wallet object links
[**store_on_chain_wallets_remove_on_chain_wallet_object**](StoreWalletOnChainApi.md#store_on_chain_wallets_remove_on_chain_wallet_object) | **DELETE** /api/v1/stores/{storeId}/payment-methods/{paymentMethodId}/wallet/objects/{objectType}/{objectId} | Remove store on-chain wallet objects
[**store_on_chain_wallets_show_on_chain_wallet_histogram**](StoreWalletOnChainApi.md#store_on_chain_wallets_show_on_chain_wallet_histogram) | **GET** /api/v1/stores/{storeId}/payment-methods/{paymentMethodId}/wallet/histogram | Get store on-chain wallet balance histogram
[**store_on_chain_wallets_show_on_chain_wallet_overview**](StoreWalletOnChainApi.md#store_on_chain_wallets_show_on_chain_wallet_overview) | **GET** /api/v1/stores/{storeId}/payment-methods/{paymentMethodId}/wallet | Get store on-chain wallet overview
[**store_on_chain_wallets_show_on_chain_wallet_transactions**](StoreWalletOnChainApi.md#store_on_chain_wallets_show_on_chain_wallet_transactions) | **GET** /api/v1/stores/{storeId}/payment-methods/{paymentMethodId}/wallet/transactions | Get store on-chain wallet transactions
[**store_on_chain_wallets_un_reserve_on_chain_wallet_receive_address**](StoreWalletOnChainApi.md#store_on_chain_wallets_un_reserve_on_chain_wallet_receive_address) | **DELETE** /api/v1/stores/{storeId}/payment-methods/{paymentMethodId}/wallet/address | UnReserve last store on-chain wallet address



## store_on_chain_payment_methods_generate_on_chain_wallet

> models::StoreOnChainPaymentMethodsGenerateOnChainWallet200Response store_on_chain_payment_methods_generate_on_chain_wallet(payment_method_id, store_id, generate_on_chain_wallet_request)
Generate store on-chain wallet

Generate a wallet and update the specified store's payment method to it

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**payment_method_id** | **String** | The payment method id of the payment method to update | [required] |
**store_id** | **String** | The store ID | [required] |
**generate_on_chain_wallet_request** | [**GenerateOnChainWalletRequest**](GenerateOnChainWalletRequest.md) |  | [required] |

### Return type

[**models::StoreOnChainPaymentMethodsGenerateOnChainWallet200Response**](StoreOnChainPaymentMethods_GenerateOnChainWallet_200_response.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_on_chain_payment_methods_get_on_chain_payment_method_preview

> models::OnChainPaymentMethodPreviewResultData store_on_chain_payment_methods_get_on_chain_payment_method_preview(store_id, payment_method_id, offset, count)
Preview store on-chain payment method addresses

View addresses of the current payment method of the store

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_id** | **String** | The store ID | [required] |
**payment_method_id** | **String** | The payment method id of the payment method to update | [required] |
**offset** | Option<**f64**> | From which index to fetch the addresses |  |
**count** | Option<**f64**> | Number of addresses to preview |  |

### Return type

[**models::OnChainPaymentMethodPreviewResultData**](OnChainPaymentMethodPreviewResultData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_on_chain_payment_methods_poston_chain_payment_method_preview

> models::OnChainPaymentMethodPreviewResultData store_on_chain_payment_methods_poston_chain_payment_method_preview(payment_method_id, store_id, store_on_chain_payment_methods_poston_chain_payment_method_preview_request, offset, count)
Preview proposed store on-chain payment method addresses

View addresses of a proposed payment method of the store

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**payment_method_id** | **String** | The payment method id of the payment method to update | [required] |
**store_id** | **String** | The store ID | [required] |
**store_on_chain_payment_methods_poston_chain_payment_method_preview_request** | [**StoreOnChainPaymentMethodsPostonChainPaymentMethodPreviewRequest**](StoreOnChainPaymentMethodsPostonChainPaymentMethodPreviewRequest.md) |  | [required] |
**offset** | Option<**f64**> | From which index to fetch the addresses |  |
**count** | Option<**f64**> | Number of addresses to preview |  |

### Return type

[**models::OnChainPaymentMethodPreviewResultData**](OnChainPaymentMethodPreviewResultData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_on_chain_wallets_add_or_update_on_chain_wallet_link

> store_on_chain_wallets_add_or_update_on_chain_wallet_link(payment_method_id, store_id, object_id, object_type, add_on_chain_wallet_object_link_request)
Add/Update store on-chain wallet object link

Add/Update wallet object link

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**payment_method_id** | **String** | The payment method id of the payment method to update | [required] |
**store_id** | **String** | The store ID | [required] |
**object_id** | **String** | The object id to fetch | [required] |
**object_type** | **String** | The object type to fetch | [required] |
**add_on_chain_wallet_object_link_request** | [**AddOnChainWalletObjectLinkRequest**](AddOnChainWalletObjectLinkRequest.md) |  | [required] |

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_on_chain_wallets_add_or_update_on_chain_wallet_objects

> models::OnChainWalletObjectData store_on_chain_wallets_add_or_update_on_chain_wallet_objects(payment_method_id, store_id, on_chain_wallet_object_data)
Add/Update store on-chain wallet objects

Add/Update wallet objects

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**payment_method_id** | **String** | The payment method id of the payment method to update | [required] |
**store_id** | **String** | The store ID | [required] |
**on_chain_wallet_object_data** | [**OnChainWalletObjectData**](OnChainWalletObjectData.md) |  | [required] |

### Return type

[**models::OnChainWalletObjectData**](OnChainWalletObjectData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_on_chain_wallets_create_on_chain_transaction

> models::StoreOnChainWalletsCreateOnChainTransaction200Response store_on_chain_wallets_create_on_chain_transaction(payment_method_id, store_id, create_on_chain_transaction_request)
Create store on-chain wallet transaction

Create store on-chain wallet transaction

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**payment_method_id** | **String** | The payment method id of the payment method to update | [required] |
**store_id** | **String** | The store ID | [required] |
**create_on_chain_transaction_request** | [**CreateOnChainTransactionRequest**](CreateOnChainTransactionRequest.md) |  | [required] |

### Return type

[**models::StoreOnChainWalletsCreateOnChainTransaction200Response**](StoreOnChainWallets_CreateOnChainTransaction_200_response.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_on_chain_wallets_get_on_chain_fee_rate

> models::OnChainWalletFeeRateData store_on_chain_wallets_get_on_chain_fee_rate(payment_method_id, store_id, block_target)
Get store on-chain wallet fee rate

Get wallet onchain fee rate

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**payment_method_id** | **String** | The payment method id of the payment method to update | [required] |
**store_id** | **String** | The store ID | [required] |
**block_target** | Option<**f64**> | The number of blocks away you are willing to target for confirmation. Defaults to the wallet's configured `RecommendedFeeBlockTarget` |  |

### Return type

[**models::OnChainWalletFeeRateData**](OnChainWalletFeeRateData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_on_chain_wallets_get_on_chain_wallet_object

> models::OnChainWalletObjectData store_on_chain_wallets_get_on_chain_wallet_object(payment_method_id, store_id, object_id, object_type, include_neighbour_data)
Get store on-chain wallet object

View wallet object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**payment_method_id** | **String** | The payment method id of the payment method to update | [required] |
**store_id** | **String** | The store ID | [required] |
**object_id** | **String** | The object id to fetch | [required] |
**object_type** | **String** | The object type to fetch | [required] |
**include_neighbour_data** | Option<**bool**> | Whether or not you should include neighbour's node data in the result (ie, `links.objectData`) |  |[default to true]

### Return type

[**models::OnChainWalletObjectData**](OnChainWalletObjectData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_on_chain_wallets_get_on_chain_wallet_objects

> Vec<models::OnChainWalletObjectData> store_on_chain_wallets_get_on_chain_wallet_objects(payment_method_id, store_id, ids, r#type, include_neighbour_data)
Get store on-chain wallet objects

View wallet objects

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**payment_method_id** | **String** | The payment method id of the payment method to update | [required] |
**store_id** | **String** | The store ID | [required] |
**ids** | Option<[**Vec<String>**](String.md)> | The ids of objects to fetch, if used, type should be specified |  |
**r#type** | Option<**String**> | The type of object to fetch |  |
**include_neighbour_data** | Option<**bool**> | Whether or not you should include neighbour's node data in the result (ie, `links.objectData`) |  |[default to true]

### Return type

[**Vec<models::OnChainWalletObjectData>**](OnChainWalletObjectData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_on_chain_wallets_get_on_chain_wallet_receive_address

> models::OnChainWalletAddressData store_on_chain_wallets_get_on_chain_wallet_receive_address(payment_method_id, store_id, force_generate)
Get store on-chain wallet address

Get or generate address for wallet

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**payment_method_id** | **String** | The payment method id of the payment method to update | [required] |
**store_id** | **String** | The store ID | [required] |
**force_generate** | Option<**bool**> | Whether to generate a new address for this request even if the previous one was not used |  |[default to false]

### Return type

[**models::OnChainWalletAddressData**](OnChainWalletAddressData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_on_chain_wallets_get_on_chain_wallet_transaction

> models::OnChainWalletTransactionData store_on_chain_wallets_get_on_chain_wallet_transaction(payment_method_id, store_id, transaction_id)
Get store on-chain wallet transaction

Get store on-chain wallet transaction

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**payment_method_id** | **String** | The payment method id of the payment method to update | [required] |
**store_id** | **String** | The store ID | [required] |
**transaction_id** | **String** | The transaction id to fetch | [required] |

### Return type

[**models::OnChainWalletTransactionData**](OnChainWalletTransactionData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_on_chain_wallets_get_on_chain_wallet_utxos

> Vec<models::OnChainWalletUtxoData> store_on_chain_wallets_get_on_chain_wallet_utxos(payment_method_id, store_id)
Get store on-chain wallet UTXOS

Get store on-chain wallet utxos

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**payment_method_id** | **String** | The payment method id of the payment method to update | [required] |
**store_id** | **String** | The store ID | [required] |

### Return type

[**Vec<models::OnChainWalletUtxoData>**](OnChainWalletUTXOData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_on_chain_wallets_patch_on_chain_wallet_transaction

> models::OnChainWalletTransactionData store_on_chain_wallets_patch_on_chain_wallet_transaction(payment_method_id, store_id, transaction_id, patch_on_chain_transaction_request, force)
Patch store on-chain wallet transaction info

Patch store on-chain wallet transaction info

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**payment_method_id** | **String** | The payment method id of the payment method to update | [required] |
**store_id** | **String** | The store ID | [required] |
**transaction_id** | **String** | The transaction id to fetch | [required] |
**patch_on_chain_transaction_request** | [**PatchOnChainTransactionRequest**](PatchOnChainTransactionRequest.md) |  | [required] |
**force** | Option<**String**> | Whether to update the label/comments even if the transaction does not yet exist |  |

### Return type

[**models::OnChainWalletTransactionData**](OnChainWalletTransactionData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_on_chain_wallets_remove_on_chain_wallet_link

> store_on_chain_wallets_remove_on_chain_wallet_link(payment_method_id, store_id, link_id, object_id, link_type, object_type)
Remove store on-chain wallet object links

Remove wallet object link

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**payment_method_id** | **String** | The payment method id of the payment method to update | [required] |
**store_id** | **String** | The store ID | [required] |
**link_id** | **String** | The object id of the linked neighbour | [required] |
**object_id** | **String** | The object id to fetch | [required] |
**link_type** | **String** | The object type of the linked neighbour | [required] |
**object_type** | **String** | The object type to fetch | [required] |

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_on_chain_wallets_remove_on_chain_wallet_object

> store_on_chain_wallets_remove_on_chain_wallet_object(payment_method_id, store_id, object_id, object_type)
Remove store on-chain wallet objects

Remove wallet object

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**payment_method_id** | **String** | The payment method id of the payment method to update | [required] |
**store_id** | **String** | The store ID | [required] |
**object_id** | **String** | The object id to fetch | [required] |
**object_type** | **String** | The object type to fetch | [required] |

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_on_chain_wallets_show_on_chain_wallet_histogram

> models::HistogramData store_on_chain_wallets_show_on_chain_wallet_histogram(payment_method_id, store_id)
Get store on-chain wallet balance histogram

View the balance histogram of the specified wallet

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**payment_method_id** | **String** | The payment method id of the payment method to update | [required] |
**store_id** | **String** | The store ID | [required] |

### Return type

[**models::HistogramData**](HistogramData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_on_chain_wallets_show_on_chain_wallet_overview

> models::OnChainWalletOverviewData store_on_chain_wallets_show_on_chain_wallet_overview(payment_method_id, store_id)
Get store on-chain wallet overview

View information about the specified wallet

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**payment_method_id** | **String** | The payment method id of the payment method to update | [required] |
**store_id** | **String** | The store ID | [required] |

### Return type

[**models::OnChainWalletOverviewData**](OnChainWalletOverviewData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_on_chain_wallets_show_on_chain_wallet_transactions

> Vec<models::OnChainWalletTransactionData> store_on_chain_wallets_show_on_chain_wallet_transactions(payment_method_id, store_id, label_filter, limit, skip, status_filter)
Get store on-chain wallet transactions

Get store on-chain wallet transactions

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**payment_method_id** | **String** | The payment method id of the payment method to update | [required] |
**store_id** | **String** | The store ID | [required] |
**label_filter** | Option<**String**> | Transaction label to filter by |  |
**limit** | Option<**i32**> | Maximum number of transactions to return |  |
**skip** | Option<**i32**> | Number of transactions to skip from the start |  |
**status_filter** | Option<[**Vec<models::TransactionStatus>**](models::TransactionStatus.md)> | Statuses to filter the transactions with |  |

### Return type

[**Vec<models::OnChainWalletTransactionData>**](OnChainWalletTransactionData.md)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_on_chain_wallets_un_reserve_on_chain_wallet_receive_address

> store_on_chain_wallets_un_reserve_on_chain_wallet_receive_address(payment_method_id, store_id)
UnReserve last store on-chain wallet address

UnReserve address

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**payment_method_id** | **String** | The payment method id of the payment method to update | [required] |
**store_id** | **String** | The store ID | [required] |

### Return type

 (empty response body)

### Authorization

[Basic](../README.md#Basic), [API_Key](../README.md#API_Key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

