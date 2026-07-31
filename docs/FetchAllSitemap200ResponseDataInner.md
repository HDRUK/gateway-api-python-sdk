# FetchAllSitemap200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**collections** | **List[List[object]]** |  | [optional] 
**data_custodians** | **List[List[object]]** |  | [optional] 
**data_custodian_networks** | **List[List[object]]** |  | [optional] 
**data_sets** | **List[List[object]]** |  | [optional] 
**durs** | **List[List[object]]** |  | [optional] 
**tools** | **List[List[object]]** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_all_sitemap200_response_data_inner import FetchAllSitemap200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of FetchAllSitemap200ResponseDataInner from a JSON string
fetch_all_sitemap200_response_data_inner_instance = FetchAllSitemap200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(FetchAllSitemap200ResponseDataInner.to_json())

# convert the object into a dict
fetch_all_sitemap200_response_data_inner_dict = fetch_all_sitemap200_response_data_inner_instance.to_dict()
# create an instance of FetchAllSitemap200ResponseDataInner from a dict
fetch_all_sitemap200_response_data_inner_from_dict = FetchAllSitemap200ResponseDataInner.from_dict(fetch_all_sitemap200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


