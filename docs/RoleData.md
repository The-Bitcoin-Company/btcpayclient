# RoleData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | Option<**String**> | The role's Id (Same as role if the role is created at server level, if the role is created at the store level the format is `STOREID::ROLE`) | [optional]
**role** | Option<**String**> | The role's name | [optional]
**permissions** | Option<**Vec<String>**> | The permissions attached to this role | [optional]
**is_server_role** | Option<**bool**> | Whether this role is at the scope of the store or scope of the server | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


