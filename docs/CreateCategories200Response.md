# CreateCategories200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | **int** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_categories200_response import CreateCategories200Response

# TODO update the JSON string below
json = "{}"
# create an instance of CreateCategories200Response from a JSON string
create_categories200_response_instance = CreateCategories200Response.from_json(json)
# print the JSON string representation of the object
print(CreateCategories200Response.to_json())

# convert the object into a dict
create_categories200_response_dict = create_categories200_response_instance.to_dict()
# create an instance of CreateCategories200Response from a dict
create_categories200_response_from_dict = CreateCategories200Response.from_dict(create_categories200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


