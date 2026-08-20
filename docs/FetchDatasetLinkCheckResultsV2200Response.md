# FetchDatasetLinkCheckResultsV2200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | **List[List[object]]** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_dataset_link_check_results_v2200_response import FetchDatasetLinkCheckResultsV2200Response

# TODO update the JSON string below
json = "{}"
# create an instance of FetchDatasetLinkCheckResultsV2200Response from a JSON string
fetch_dataset_link_check_results_v2200_response_instance = FetchDatasetLinkCheckResultsV2200Response.from_json(json)
# print the JSON string representation of the object
print(FetchDatasetLinkCheckResultsV2200Response.to_json())

# convert the object into a dict
fetch_dataset_link_check_results_v2200_response_dict = fetch_dataset_link_check_results_v2200_response_instance.to_dict()
# create an instance of FetchDatasetLinkCheckResultsV2200Response from a dict
fetch_dataset_link_check_results_v2200_response_from_dict = FetchDatasetLinkCheckResultsV2200Response.from_dict(fetch_dataset_link_check_results_v2200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


