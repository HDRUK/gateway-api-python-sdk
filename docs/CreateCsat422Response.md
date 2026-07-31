# CreateCsat422Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**id** | **int** |  | [optional] 
**errors** | **object** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_csat422_response import CreateCsat422Response

# TODO update the JSON string below
json = "{}"
# create an instance of CreateCsat422Response from a JSON string
create_csat422_response_instance = CreateCsat422Response.from_json(json)
# print the JSON string representation of the object
print(CreateCsat422Response.to_json())

# convert the object into a dict
create_csat422_response_dict = create_csat422_response_instance.to_dict()
# create an instance of CreateCsat422Response from a dict
create_csat422_response_from_dict = CreateCsat422Response.from_dict(create_csat422_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


