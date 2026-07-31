# EditCsatRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reason** | **str** |  | 
**score** | **int** |  | 

## Example

```python
from gateway_api_sdk.models.edit_csat_request import EditCsatRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EditCsatRequest from a JSON string
edit_csat_request_instance = EditCsatRequest.from_json(json)
# print the JSON string representation of the object
print(EditCsatRequest.to_json())

# convert the object into a dict
edit_csat_request_dict = edit_csat_request_instance.to_dict()
# create an instance of EditCsatRequest from a dict
edit_csat_request_from_dict = EditCsatRequest.from_dict(edit_csat_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


