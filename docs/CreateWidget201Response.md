# CreateWidget201Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | **object** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_widget201_response import CreateWidget201Response

# TODO update the JSON string below
json = "{}"
# create an instance of CreateWidget201Response from a JSON string
create_widget201_response_instance = CreateWidget201Response.from_json(json)
# print the JSON string representation of the object
print(CreateWidget201Response.to_json())

# convert the object into a dict
create_widget201_response_dict = create_widget201_response_instance.to_dict()
# create an instance of CreateWidget201Response from a dict
create_widget201_response_from_dict = CreateWidget201Response.from_dict(create_widget201_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


