# OnChainWalletObjectLink

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**r#type** | Option<**String**> | The type of wallet object | [optional]
**id** | Option<**String**> | The identifier of the wallet object (unique per type, per wallet) | [optional]
**link_data** | Option<[**std::collections::HashMap<String, serde_json::Value>**](serde_json::Value.md)> | The data of the link | [optional]
**object_data** | Option<[**std::collections::HashMap<String, serde_json::Value>**](serde_json::Value.md)> | The data of the neighbour's node (`null` if there isn't any data or `includeNeighbourData` is `false`) | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


