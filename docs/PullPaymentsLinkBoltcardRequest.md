# PullPaymentsLinkBoltcardRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**uid** | **String** | The `UID` of the NTag424 | 
**on_existing** | Option<**String**> | What to do if the boltcard is already linked.  * `KeepVersion` will return the keys (K0-K4) that are already registered.  * `UpdateVersion` will increment the version of the key, and thus return different keys (K0-K4). (See [Deterministic Boltcard Key Generation](https://github.com/boltcard/boltcard/blob/main/docs/DETERMINISTIC.md)) | [optional][default to UpdateVersion]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


