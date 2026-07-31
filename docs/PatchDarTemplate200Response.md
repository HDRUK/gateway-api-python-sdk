# PatchDarTemplate200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**PatchDarTemplate200ResponseData**](PatchDarTemplate200ResponseData.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.patch_dar_template200_response import PatchDarTemplate200Response

# TODO update the JSON string below
json = "{}"
# create an instance of PatchDarTemplate200Response from a JSON string
patch_dar_template200_response_instance = PatchDarTemplate200Response.from_json(json)
# print the JSON string representation of the object
print(PatchDarTemplate200Response.to_json())

# convert the object into a dict
patch_dar_template200_response_dict = patch_dar_template200_response_instance.to_dict()
# create an instance of PatchDarTemplate200Response from a dict
patch_dar_template200_response_from_dict = PatchDarTemplate200Response.from_dict(patch_dar_template200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


