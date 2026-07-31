# CreateTypeCategoriesRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**description** | **str** |  | [optional] 
**enabled** | **bool** |  | 

## Example

```python
from gateway_api_sdk.models.create_type_categories_request import CreateTypeCategoriesRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateTypeCategoriesRequest from a JSON string
create_type_categories_request_instance = CreateTypeCategoriesRequest.from_json(json)
# print the JSON string representation of the object
print(CreateTypeCategoriesRequest.to_json())

# convert the object into a dict
create_type_categories_request_dict = create_type_categories_request_instance.to_dict()
# create an instance of CreateTypeCategoriesRequest from a dict
create_type_categories_request_from_dict = CreateTypeCategoriesRequest.from_dict(create_type_categories_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


