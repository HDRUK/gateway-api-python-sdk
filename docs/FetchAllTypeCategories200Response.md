# FetchAllTypeCategories200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**List[TypeCategory]**](TypeCategory.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_all_type_categories200_response import FetchAllTypeCategories200Response

# TODO update the JSON string below
json = "{}"
# create an instance of FetchAllTypeCategories200Response from a JSON string
fetch_all_type_categories200_response_instance = FetchAllTypeCategories200Response.from_json(json)
# print the JSON string representation of the object
print(FetchAllTypeCategories200Response.to_json())

# convert the object into a dict
fetch_all_type_categories200_response_dict = fetch_all_type_categories200_response_instance.to_dict()
# create an instance of FetchAllTypeCategories200Response from a dict
fetch_all_type_categories200_response_from_dict = FetchAllTypeCategories200Response.from_dict(fetch_all_type_categories200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


