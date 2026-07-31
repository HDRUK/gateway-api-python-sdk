# UpdateTypeCategoriesRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**description** | **str** |  | [optional] 
**enabled** | **str** |  | 

## Example

```python
from gateway_api_sdk.models.update_type_categories_request import UpdateTypeCategoriesRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateTypeCategoriesRequest from a JSON string
update_type_categories_request_instance = UpdateTypeCategoriesRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateTypeCategoriesRequest.to_json())

# convert the object into a dict
update_type_categories_request_dict = update_type_categories_request_instance.to_dict()
# create an instance of UpdateTypeCategoriesRequest from a dict
update_type_categories_request_from_dict = UpdateTypeCategoriesRequest.from_dict(update_type_categories_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


