# UpdateLibraries200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**UpdateLibraries200ResponseData**](UpdateLibraries200ResponseData.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.update_libraries200_response import UpdateLibraries200Response

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateLibraries200Response from a JSON string
update_libraries200_response_instance = UpdateLibraries200Response.from_json(json)
# print the JSON string representation of the object
print(UpdateLibraries200Response.to_json())

# convert the object into a dict
update_libraries200_response_dict = update_libraries200_response_instance.to_dict()
# create an instance of UpdateLibraries200Response from a dict
update_libraries200_response_from_dict = UpdateLibraries200Response.from_dict(update_libraries200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


