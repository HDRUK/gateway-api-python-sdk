# FetchDataProviderColls200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**deleted_at** | **datetime** |  | [optional] 
**name** | **str** |  | [optional] 
**summary** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**service** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_data_provider_colls200_response_data_inner import FetchDataProviderColls200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of FetchDataProviderColls200ResponseDataInner from a JSON string
fetch_data_provider_colls200_response_data_inner_instance = FetchDataProviderColls200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(FetchDataProviderColls200ResponseDataInner.to_json())

# convert the object into a dict
fetch_data_provider_colls200_response_data_inner_dict = fetch_data_provider_colls200_response_data_inner_instance.to_dict()
# create an instance of FetchDataProviderColls200ResponseDataInner from a dict
fetch_data_provider_colls200_response_data_inner_from_dict = FetchDataProviderColls200ResponseDataInner.from_dict(fetch_data_provider_colls200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


