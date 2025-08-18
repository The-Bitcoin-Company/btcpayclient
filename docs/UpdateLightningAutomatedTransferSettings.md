# UpdateLightningAutomatedTransferSettings

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**interval_seconds** | Option<[**models::TimeSpanSeconds**](serde_json::Value.md)> | How often should the processor run | [optional]
**cancel_payout_after_failures** | Option<**f64**> | How many failures should the processor tolerate before cancelling the payout | [optional]
**process_new_payouts_instantly** | Option<**bool**> | Skip the interval when ane eligible payout has been approved (or created with pre-approval) | [optional][default to false]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


