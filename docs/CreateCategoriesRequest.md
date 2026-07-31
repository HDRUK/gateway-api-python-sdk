# CreateCategoriesRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**enabled** | **bool** |  | 

## Example

```python
from gateway_api_sdk.models.create_categories_request import CreateCategoriesRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateCategoriesRequest from a JSON string
create_categories_request_instance = CreateCategoriesRequest.from_json(json)
# print the JSON string representation of the object
print(CreateCategoriesRequest.to_json())

# convert the object into a dict
create_categories_request_dict = create_categories_request_instance.to_dict()
# create an instance of CreateCategoriesRequest from a dict
create_categories_request_from_dict = CreateCategoriesRequest.from_dict(create_categories_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


