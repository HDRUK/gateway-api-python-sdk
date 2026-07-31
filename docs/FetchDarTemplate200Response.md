# FetchDarTemplate200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**FetchDarTemplates200ResponseDataInner**](FetchDarTemplates200ResponseDataInner.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_dar_template200_response import FetchDarTemplate200Response

# TODO update the JSON string below
json = "{}"
# create an instance of FetchDarTemplate200Response from a JSON string
fetch_dar_template200_response_instance = FetchDarTemplate200Response.from_json(json)
# print the JSON string representation of the object
print(FetchDarTemplate200Response.to_json())

# convert the object into a dict
fetch_dar_template200_response_dict = fetch_dar_template200_response_instance.to_dict()
# create an instance of FetchDarTemplate200Response from a dict
fetch_dar_template200_response_from_dict = FetchDarTemplate200Response.from_dict(fetch_dar_template200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


