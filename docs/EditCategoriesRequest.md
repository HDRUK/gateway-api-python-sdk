# EditCategoriesRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**enabled** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.edit_categories_request import EditCategoriesRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EditCategoriesRequest from a JSON string
edit_categories_request_instance = EditCategoriesRequest.from_json(json)
# print the JSON string representation of the object
print(EditCategoriesRequest.to_json())

# convert the object into a dict
edit_categories_request_dict = edit_categories_request_instance.to_dict()
# create an instance of EditCategoriesRequest from a dict
edit_categories_request_from_dict = EditCategoriesRequest.from_dict(edit_categories_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


