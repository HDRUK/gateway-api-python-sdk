# FetchDatasetViewsTopV3200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**FetchDatasetViewsTopV3200ResponseData**](FetchDatasetViewsTopV3200ResponseData.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_dataset_views_top_v3200_response import FetchDatasetViewsTopV3200Response

# TODO update the JSON string below
json = "{}"
# create an instance of FetchDatasetViewsTopV3200Response from a JSON string
fetch_dataset_views_top_v3200_response_instance = FetchDatasetViewsTopV3200Response.from_json(json)
# print the JSON string representation of the object
print(FetchDatasetViewsTopV3200Response.to_json())

# convert the object into a dict
fetch_dataset_views_top_v3200_response_dict = fetch_dataset_views_top_v3200_response_instance.to_dict()
# create an instance of FetchDatasetViewsTopV3200Response from a dict
fetch_dataset_views_top_v3200_response_from_dict = FetchDatasetViewsTopV3200Response.from_dict(fetch_dataset_views_top_v3200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


