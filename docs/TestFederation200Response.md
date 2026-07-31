# TestFederation200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **bool** |  | [optional] 
**errors** | **str** |  | [optional] 
**status** | **int** |  | [optional] 
**title** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.test_federation200_response import TestFederation200Response

# TODO update the JSON string below
json = "{}"
# create an instance of TestFederation200Response from a JSON string
test_federation200_response_instance = TestFederation200Response.from_json(json)
# print the JSON string representation of the object
print(TestFederation200Response.to_json())

# convert the object into a dict
test_federation200_response_dict = test_federation200_response_instance.to_dict()
# create an instance of TestFederation200Response from a dict
test_federation200_response_from_dict = TestFederation200Response.from_dict(test_federation200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


