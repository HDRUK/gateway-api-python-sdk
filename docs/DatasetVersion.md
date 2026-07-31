# DatasetVersion

A versioned snapshot of dataset metadata in GWDM format

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**dataset_id** | **int** |  | [optional] 
**version** | **int** |  | [optional] 
**title** | **str** |  | [optional] 
**short_title** | **str** |  | [optional] 
**metadata** | **object** | Full GWDM-format metadata document for this version | [optional] 
**patch** | **List[object]** | RFC 6902 JSON Patch array used to reconstruct this version from the previous snapshot. Null for full snapshots (v1 and every 10th version). | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.dataset_version import DatasetVersion

# TODO update the JSON string below
json = "{}"
# create an instance of DatasetVersion from a JSON string
dataset_version_instance = DatasetVersion.from_json(json)
# print the JSON string representation of the object
print(DatasetVersion.to_json())

# convert the object into a dict
dataset_version_dict = dataset_version_instance.to_dict()
# create an instance of DatasetVersion from a dict
dataset_version_from_dict = DatasetVersion.from_dict(dataset_version_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


