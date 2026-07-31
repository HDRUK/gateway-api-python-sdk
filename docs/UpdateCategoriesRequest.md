# UpdateCategoriesRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**enabled** | **str** |  | 

## Example

```python
from gateway_api_sdk.models.update_categories_request import UpdateCategoriesRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateCategoriesRequest from a JSON string
update_categories_request_instance = UpdateCategoriesRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateCategoriesRequest.to_json())

# convert the object into a dict
update_categories_request_dict = update_categories_request_instance.to_dict()
# create an instance of UpdateCategoriesRequest from a dict
update_categories_request_from_dict = UpdateCategoriesRequest.from_dict(update_categories_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


