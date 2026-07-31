# PatchDatasetsV2Request


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**create_origin** | **str** |  | [optional] 
**metadata** | **object** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.patch_datasets_v2_request import PatchDatasetsV2Request

# TODO update the JSON string below
json = "{}"
# create an instance of PatchDatasetsV2Request from a JSON string
patch_datasets_v2_request_instance = PatchDatasetsV2Request.from_json(json)
# print the JSON string representation of the object
print(PatchDatasetsV2Request.to_json())

# convert the object into a dict
patch_datasets_v2_request_dict = patch_datasets_v2_request_instance.to_dict()
# create an instance of PatchDatasetsV2Request from a dict
patch_datasets_v2_request_from_dict = PatchDatasetsV2Request.from_dict(patch_datasets_v2_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


