# Model02ada355a680c816624e98ae028dc8b6Request


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**summary** | **str** |  | 
**enabled** | **bool** |  | 
**service** | **str** |  | [optional] 
**team_ids** | **List[int]** |  | 

## Example

```python
from gateway_api_sdk.models.model02ada355a680c816624e98ae028dc8b6_request import Model02ada355a680c816624e98ae028dc8b6Request

# TODO update the JSON string below
json = "{}"
# create an instance of Model02ada355a680c816624e98ae028dc8b6Request from a JSON string
model02ada355a680c816624e98ae028dc8b6_request_instance = Model02ada355a680c816624e98ae028dc8b6Request.from_json(json)
# print the JSON string representation of the object
print(Model02ada355a680c816624e98ae028dc8b6Request.to_json())

# convert the object into a dict
model02ada355a680c816624e98ae028dc8b6_request_dict = model02ada355a680c816624e98ae028dc8b6_request_instance.to_dict()
# create an instance of Model02ada355a680c816624e98ae028dc8b6Request from a dict
model02ada355a680c816624e98ae028dc8b6_request_from_dict = Model02ada355a680c816624e98ae028dc8b6Request.from_dict(model02ada355a680c816624e98ae028dc8b6_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


