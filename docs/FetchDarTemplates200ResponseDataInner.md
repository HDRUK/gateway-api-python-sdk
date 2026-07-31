# FetchDarTemplates200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**deleted_at** | **datetime** |  | [optional] 
**team_id** | **int** |  | [optional] 
**user_id** | **int** |  | [optional] 
**published** | **bool** |  | [optional] 
**locked** | **bool** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_dar_templates200_response_data_inner import FetchDarTemplates200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of FetchDarTemplates200ResponseDataInner from a JSON string
fetch_dar_templates200_response_data_inner_instance = FetchDarTemplates200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(FetchDarTemplates200ResponseDataInner.to_json())

# convert the object into a dict
fetch_dar_templates200_response_data_inner_dict = fetch_dar_templates200_response_data_inner_instance.to_dict()
# create an instance of FetchDarTemplates200ResponseDataInner from a dict
fetch_dar_templates200_response_data_inner_from_dict = FetchDarTemplates200ResponseDataInner.from_dict(fetch_dar_templates200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


