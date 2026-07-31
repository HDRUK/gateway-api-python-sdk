# FetchDataProviderCollSummary200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**name** | **str** |  | [optional] 
**img_url** | **str** |  | [optional] 
**url** | **str** |  | [optional] 
**summary** | **str** |  | [optional] 
**datasets** | **List[object]** |  | [optional] 
**durs** | **List[object]** |  | [optional] 
**tools** | **List[object]** |  | [optional] 
**publications** | **List[object]** |  | [optional] 
**collections** | **List[object]** |  | [optional] 
**service** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_data_provider_coll_summary200_response_data import FetchDataProviderCollSummary200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of FetchDataProviderCollSummary200ResponseData from a JSON string
fetch_data_provider_coll_summary200_response_data_instance = FetchDataProviderCollSummary200ResponseData.from_json(json)
# print the JSON string representation of the object
print(FetchDataProviderCollSummary200ResponseData.to_json())

# convert the object into a dict
fetch_data_provider_coll_summary200_response_data_dict = fetch_data_provider_coll_summary200_response_data_instance.to_dict()
# create an instance of FetchDataProviderCollSummary200ResponseData from a dict
fetch_data_provider_coll_summary200_response_data_from_dict = FetchDataProviderCollSummary200ResponseData.from_dict(fetch_data_provider_coll_summary200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


