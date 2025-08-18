# UsersCreateUserRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email** | Option<**String**> | The email of the new user | [optional]
**name** | Option<**String**> | The name of the new user | [optional]
**image_url** | Option<**String**> | The profile picture URL of the new user | [optional]
**password** | Option<**String**> | The password of the new user (if no password is set, an email will be sent to the user requiring him to set the password) | [optional]
**is_administrator** | Option<**bool**> | Make this user administrator (only if you have the `unrestricted` permission of a server administrator) | [optional][default to false]
**send_invitation_email** | Option<**bool**> | Flag to specify if an email invitation should be sent to the user | [optional][default to true]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


