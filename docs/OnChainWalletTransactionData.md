# OnChainWalletTransactionData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**transaction_hash** | Option<**String**> | The transaction id | [optional]
**comment** | Option<**String**> | A comment linked to the transaction | [optional]
**amount** | Option<**String**> | The amount the wallet balance changed with this transaction | [optional]
**block_hash** | Option<**String**> | The hash of the block that confirmed this transaction. Null if still unconfirmed. | [optional]
**block_height** | Option<**String**> | The height of the block that confirmed this transaction. Null if still unconfirmed. | [optional]
**confirmations** | Option<**String**> | The number of confirmations for this transaction | [optional]
**timestamp** | Option<**f64**> | The time of the transaction | [optional]
**status** | Option<[**models::TransactionStatus**](TransactionStatus.md)> | The status of this transaction | [optional]
**labels** | Option<[**Vec<models::LabelData>**](LabelData.md)> | Labels linked to this transaction | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


