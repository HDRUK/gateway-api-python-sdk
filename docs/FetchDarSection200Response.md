# FetchDarSection200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**FetchDarSections200ResponseDataInner**](FetchDarSections200ResponseDataInner.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_dar_section200_response import FetchDarSection200Response

# TODO update the JSON string below
json = "{}"
# create an instance of FetchDarSection200Response from a JSON string
fetch_dar_section200_response_instance = FetchDarSection200Response.from_json(json)
# print the JSON string representation of the object
print(FetchDarSection200Response.to_json())

# convert the object into a dict
fetch_dar_section200_response_dict = fetch_dar_section200_response_instance.to_dict()
# create an instance of FetchDarSection200Response from a dict
fetch_dar_section200_response_from_dict = FetchDarSection200Response.from_dict(fetch_dar_section200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


