# CreateDatasetsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**team_id** | **int** |  | [optional] 
**user_id** | **int** |  | [optional] 
**create_origin** | **str** |  | [optional] 
**mongo_object_id** | **str** |  | [optional] 
**mongo_id** | **str** |  | [optional] 
**mongo_pid** | **str** |  | [optional] 
**datasetid** | **str** |  | [optional] 
**metadata** | **object** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_datasets_request import CreateDatasetsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateDatasetsRequest from a JSON string
create_datasets_request_instance = CreateDatasetsRequest.from_json(json)
# print the JSON string representation of the object
print(CreateDatasetsRequest.to_json())

# convert the object into a dict
create_datasets_request_dict = create_datasets_request_instance.to_dict()
# create an instance of CreateDatasetsRequest from a dict
create_datasets_request_from_dict = CreateDatasetsRequest.from_dict(create_datasets_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


