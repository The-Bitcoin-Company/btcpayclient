# PayoutData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | Option<**String**> | The id of the payout | [optional]
**revision** | Option<**i32**> | The revision number of the payout. This revision number is incremented when the payout amount or destination is modified before the approval. | [optional]
**pull_payment_id** | Option<**String**> | The id of the pull payment this payout belongs to | [optional]
**date** | Option<**String**> | The creation date of the payout as a unix timestamp | [optional]
**destination** | Option<**String**> | The destination of the payout (can be an address or a BIP21 url) | [optional]
**original_currency** | Option<**String**> | The currency before being converted into the payout's currency | [optional]
**original_amount** | Option<**String**> | The amount in originalCurrency before being converted into the payout's currency | [optional]
**payout_currency** | Option<**String**> | The currency of the payout after conversion. | [optional]
**payout_amount** | Option<**String**> | The amount in payoutCurrency after conversion. (This property is set after the payout has been Approved) | [optional]
**payout_method_id** | Option<**String**> | Payout method IDs. Available payment method IDs for Bitcoin are:   - `\"BTC-CHAIN\"`: Onchain    -`\"BTC-LN\"`: Lightning | [optional]
**state** | Option<[**models::PayoutState**](PayoutState.md)> |  | [optional]
**payment_proof** | Option<[**models::PayoutPaymentProof**](PayoutPaymentProof.md)> |  | [optional]
**metadata** | Option<[**models::GeneralInformation**](General_information.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


