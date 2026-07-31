# GetCancerTypeFilters200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**filter_id** | **str** |  | [optional] 
**label** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**category** | **str** |  | [optional] 
**primary_group** | **str** |  | [optional] 
**count** | **str** |  | [optional] 
**parent_id** | **int** |  | [optional] 
**level** | **int** |  | [optional] 
**children** | **List[object]** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.get_cancer_type_filters200_response_data_inner import GetCancerTypeFilters200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of GetCancerTypeFilters200ResponseDataInner from a JSON string
get_cancer_type_filters200_response_data_inner_instance = GetCancerTypeFilters200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(GetCancerTypeFilters200ResponseDataInner.to_json())

# convert the object into a dict
get_cancer_type_filters200_response_data_inner_dict = get_cancer_type_filters200_response_data_inner_instance.to_dict()
# create an instance of GetCancerTypeFilters200ResponseDataInner from a dict
get_cancer_type_filters200_response_data_inner_from_dict = GetCancerTypeFilters200ResponseDataInner.from_dict(get_cancer_type_filters200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


