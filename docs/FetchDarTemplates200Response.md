# FetchDarTemplates200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**List[FetchDarTemplates200ResponseDataInner]**](FetchDarTemplates200ResponseDataInner.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_dar_templates200_response import FetchDarTemplates200Response

# TODO update the JSON string below
json = "{}"
# create an instance of FetchDarTemplates200Response from a JSON string
fetch_dar_templates200_response_instance = FetchDarTemplates200Response.from_json(json)
# print the JSON string representation of the object
print(FetchDarTemplates200Response.to_json())

# convert the object into a dict
fetch_dar_templates200_response_dict = fetch_dar_templates200_response_instance.to_dict()
# create an instance of FetchDarTemplates200Response from a dict
fetch_dar_templates200_response_from_dict = FetchDarTemplates200Response.from_dict(fetch_dar_templates200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


