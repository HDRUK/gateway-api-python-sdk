# FetchLibraries200ResponseDataDataset


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**status** | **str** |  | [optional] 
**team** | [**FetchLibraries200ResponseDataDatasetTeam**](FetchLibraries200ResponseDataDatasetTeam.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_libraries200_response_data_dataset import FetchLibraries200ResponseDataDataset

# TODO update the JSON string below
json = "{}"
# create an instance of FetchLibraries200ResponseDataDataset from a JSON string
fetch_libraries200_response_data_dataset_instance = FetchLibraries200ResponseDataDataset.from_json(json)
# print the JSON string representation of the object
print(FetchLibraries200ResponseDataDataset.to_json())

# convert the object into a dict
fetch_libraries200_response_data_dataset_dict = fetch_libraries200_response_data_dataset_instance.to_dict()
# create an instance of FetchLibraries200ResponseDataDataset from a dict
fetch_libraries200_response_data_dataset_from_dict = FetchLibraries200ResponseDataDataset.from_dict(fetch_libraries200_response_data_dataset_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


