# UpdateCategories200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**Category**](Category.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.update_categories200_response import UpdateCategories200Response

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateCategories200Response from a JSON string
update_categories200_response_instance = UpdateCategories200Response.from_json(json)
# print the JSON string representation of the object
print(UpdateCategories200Response.to_json())

# convert the object into a dict
update_categories200_response_dict = update_categories200_response_instance.to_dict()
# create an instance of UpdateCategories200Response from a dict
update_categories200_response_from_dict = UpdateCategories200Response.from_dict(update_categories200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


