# FetchDatasets200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**Dataset**](Dataset.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_datasets200_response import FetchDatasets200Response

# TODO update the JSON string below
json = "{}"
# create an instance of FetchDatasets200Response from a JSON string
fetch_datasets200_response_instance = FetchDatasets200Response.from_json(json)
# print the JSON string representation of the object
print(FetchDatasets200Response.to_json())

# convert the object into a dict
fetch_datasets200_response_dict = fetch_datasets200_response_instance.to_dict()
# create an instance of FetchDatasets200Response from a dict
fetch_datasets200_response_from_dict = FetchDatasets200Response.from_dict(fetch_datasets200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


