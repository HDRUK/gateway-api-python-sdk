# FetchPublications200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**Publication**](Publication.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_publications200_response import FetchPublications200Response

# TODO update the JSON string below
json = "{}"
# create an instance of FetchPublications200Response from a JSON string
fetch_publications200_response_instance = FetchPublications200Response.from_json(json)
# print the JSON string representation of the object
print(FetchPublications200Response.to_json())

# convert the object into a dict
fetch_publications200_response_dict = fetch_publications200_response_instance.to_dict()
# create an instance of FetchPublications200Response from a dict
fetch_publications200_response_from_dict = FetchPublications200Response.from_dict(fetch_publications200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


