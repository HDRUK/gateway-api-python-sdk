# FetchProgrammingPackages200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**ProgrammingPackage**](ProgrammingPackage.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_programming_packages200_response import FetchProgrammingPackages200Response

# TODO update the JSON string below
json = "{}"
# create an instance of FetchProgrammingPackages200Response from a JSON string
fetch_programming_packages200_response_instance = FetchProgrammingPackages200Response.from_json(json)
# print the JSON string representation of the object
print(FetchProgrammingPackages200Response.to_json())

# convert the object into a dict
fetch_programming_packages200_response_dict = fetch_programming_packages200_response_instance.to_dict()
# create an instance of FetchProgrammingPackages200Response from a dict
fetch_programming_packages200_response_from_dict = FetchProgrammingPackages200Response.from_dict(fetch_programming_packages200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


