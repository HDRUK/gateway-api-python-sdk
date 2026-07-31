# PatchDarTemplate200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**applicant_id** | **int** |  | [optional] 
**submission_status** | **str** |  | [optional] 
**approval_status** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.patch_dar_template200_response_data import PatchDarTemplate200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of PatchDarTemplate200ResponseData from a JSON string
patch_dar_template200_response_data_instance = PatchDarTemplate200ResponseData.from_json(json)
# print the JSON string representation of the object
print(PatchDarTemplate200ResponseData.to_json())

# convert the object into a dict
patch_dar_template200_response_data_dict = patch_dar_template200_response_data_instance.to_dict()
# create an instance of PatchDarTemplate200ResponseData from a dict
patch_dar_template200_response_data_from_dict = PatchDarTemplate200ResponseData.from_dict(patch_dar_template200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


