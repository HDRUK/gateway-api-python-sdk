# Authentication200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**access_token** | **str** |  | [optional] 
**token_type** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.authentication200_response import Authentication200Response

# TODO update the JSON string below
json = "{}"
# create an instance of Authentication200Response from a JSON string
authentication200_response_instance = Authentication200Response.from_json(json)
# print the JSON string representation of the object
print(Authentication200Response.to_json())

# convert the object into a dict
authentication200_response_dict = authentication200_response_instance.to_dict()
# create an instance of Authentication200Response from a dict
authentication200_response_from_dict = Authentication200Response.from_dict(authentication200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


