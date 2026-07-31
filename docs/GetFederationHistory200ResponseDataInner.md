# GetFederationHistory200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**job_uuid** | **str** |  | [optional] 
**started_at** | **datetime** |  | [optional] 
**finished_at** | **datetime** |  | [optional] 
**status** | **str** |  | [optional] 
**message** | **str** |  | [optional] 
**failed_datasets** | [**List[GetFederationHistory200ResponseDataInnerFailedDatasetsInner]**](GetFederationHistory200ResponseDataInnerFailedDatasetsInner.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.get_federation_history200_response_data_inner import GetFederationHistory200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of GetFederationHistory200ResponseDataInner from a JSON string
get_federation_history200_response_data_inner_instance = GetFederationHistory200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(GetFederationHistory200ResponseDataInner.to_json())

# convert the object into a dict
get_federation_history200_response_data_inner_dict = get_federation_history200_response_data_inner_instance.to_dict()
# create an instance of GetFederationHistory200ResponseDataInner from a dict
get_federation_history200_response_data_inner_from_dict = GetFederationHistory200ResponseDataInner.from_dict(get_federation_history200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


