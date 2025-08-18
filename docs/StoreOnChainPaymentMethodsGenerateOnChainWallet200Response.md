# StoreOnChainPaymentMethodsGenerateOnChainWallet200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enabled** | Option<**bool**> | Whether the payment method is enabled | [optional]
**payment_method_id** | Option<**String**> | Payment method IDs. Available payment method IDs for Bitcoin are:   - `\"BTC-CHAIN\"`: Onchain    -`\"BTC-LN\"`: Lightning    - `\"BTC-LNURL\"`: LNURL | [optional]
**config** | Option<[**models::OnChainPaymentMethodBaseData**](OnChainPaymentMethodBaseData.md)> |  | [optional]
**mnemonic** | Option<**String**> | A BIP39 mnemonic | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


