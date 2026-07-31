# FetchAllDatasets200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[Dataset]**](Dataset.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_all_datasets200_response import FetchAllDatasets200Response

# TODO update the JSON string below
json = "{}"
# create an instance of FetchAllDatasets200Response from a JSON string
fetch_all_datasets200_response_instance = FetchAllDatasets200Response.from_json(json)
# print the JSON string representation of the object
print(FetchAllDatasets200Response.to_json())

# convert the object into a dict
fetch_all_datasets200_response_dict = fetch_all_datasets200_response_instance.to_dict()
# create an instance of FetchAllDatasets200Response from a dict
fetch_all_datasets200_response_from_dict = FetchAllDatasets200Response.from_dict(fetch_all_datasets200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


