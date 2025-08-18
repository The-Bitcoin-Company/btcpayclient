# UpdateOnChainAutomatedTransferSettings

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**fee_target_block** | Option<**f64**> | How many blocks should the fee rate calculation target to confirm in. Set to 1 if not provided | [optional]
**interval_seconds** | Option<[**models::TimeSpanSeconds**](serde_json::Value.md)> | How often should the processor run | [optional]
**threshold** | Option<**String**> | Only process payouts when this payout sum is reached. | [optional]
**process_new_payouts_instantly** | Option<**bool**> | Skip the interval when ane eligible payout has been approved (or created with pre-approval) | [optional][default to false]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


