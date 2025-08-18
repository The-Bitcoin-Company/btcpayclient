# ApplicationServerInfoSyncStatusData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**payment_method_id** | Option<**String**> | Payment method IDs. Available payment method IDs for Bitcoin are:   - `\"BTC-CHAIN\"`: Onchain    -`\"BTC-LN\"`: Lightning    - `\"BTC-LNURL\"`: LNURL | [optional]
**node_information** | Option<[**models::ApplicationServerInfoNodeStatusData**](ApplicationServerInfoNodeStatusData.md)> |  | [optional]
**chain_height** | Option<**i32**> | The height of the chain of header of the internal indexer | [optional]
**sync_height** | Option<**f64**> | The height of the latest indexed block of the internal indexer | [optional]
**available** | Option<**bool**> | True if the full node and the indexer are fully synchronized | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


