# FetchTypeCategories200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**TypeCategory**](TypeCategory.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_type_categories200_response import FetchTypeCategories200Response

# TODO update the JSON string below
json = "{}"
# create an instance of FetchTypeCategories200Response from a JSON string
fetch_type_categories200_response_instance = FetchTypeCategories200Response.from_json(json)
# print the JSON string representation of the object
print(FetchTypeCategories200Response.to_json())

# convert the object into a dict
fetch_type_categories200_response_dict = fetch_type_categories200_response_instance.to_dict()
# create an instance of FetchTypeCategories200Response from a dict
fetch_type_categories200_response_from_dict = FetchTypeCategories200Response.from_dict(fetch_type_categories200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


