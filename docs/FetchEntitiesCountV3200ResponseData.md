# FetchEntitiesCountV3200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**total** | **int** |  | [optional] 
**total_by_interval** | **int** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_entities_count_v3200_response_data import FetchEntitiesCountV3200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of FetchEntitiesCountV3200ResponseData from a JSON string
fetch_entities_count_v3200_response_data_instance = FetchEntitiesCountV3200ResponseData.from_json(json)
# print the JSON string representation of the object
print(FetchEntitiesCountV3200ResponseData.to_json())

# convert the object into a dict
fetch_entities_count_v3200_response_data_dict = fetch_entities_count_v3200_response_data_instance.to_dict()
# create an instance of FetchEntitiesCountV3200ResponseData from a dict
fetch_entities_count_v3200_response_data_from_dict = FetchEntitiesCountV3200ResponseData.from_dict(fetch_entities_count_v3200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


