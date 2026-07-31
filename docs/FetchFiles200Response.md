# FetchFiles200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[FetchFiles200ResponseDataInner]**](FetchFiles200ResponseDataInner.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_files200_response import FetchFiles200Response

# TODO update the JSON string below
json = "{}"
# create an instance of FetchFiles200Response from a JSON string
fetch_files200_response_instance = FetchFiles200Response.from_json(json)
# print the JSON string representation of the object
print(FetchFiles200Response.to_json())

# convert the object into a dict
fetch_files200_response_dict = fetch_files200_response_instance.to_dict()
# create an instance of FetchFiles200Response from a dict
fetch_files200_response_from_dict = FetchFiles200Response.from_dict(fetch_files200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


