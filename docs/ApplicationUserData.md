# ApplicationUserData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | Option<**String**> | The id of the user | [optional]
**email** | Option<**String**> | The email of the user | [optional]
**name** | Option<**String**> | The name of the user | [optional]
**image_url** | Option<**String**> | The profile picture URL of the user | [optional]
**invitation_url** | Option<**String**> | The pending invitation URL of the user | [optional]
**email_confirmed** | Option<**bool**> | True if the email has been confirmed by the user | [optional]
**requires_email_confirmation** | Option<**bool**> | True if the email requires confirmation to log in | [optional]
**approved** | Option<**bool**> | True if an admin has approved the user | [optional]
**requires_approval** | Option<**bool**> | True if the instance requires approval to log in | [optional]
**created** | Option<**f64**> | The creation date of the user as a unix timestamp. Null if created before v1.0.5.6 | [optional]
**disabled** | Option<**bool**> | True if an admin has disabled the user | [optional]
**roles** | Option<**Vec<String>**> | The roles of the user | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


