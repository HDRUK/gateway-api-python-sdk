# CreateDatasetsV2Request


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**team_id** | **int** |  | [optional] 
**user_id** | **int** |  | [optional] 
**create_origin** | **str** |  | [optional] 
**mongo_object_id** | **str** |  | [optional] 
**mongo_id** | **str** |  | [optional] 
**mongo_pid** | **str** |  | [optional] 
**metadata** | **object** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_datasets_v2_request import CreateDatasetsV2Request

# TODO update the JSON string below
json = "{}"
# create an instance of CreateDatasetsV2Request from a JSON string
create_datasets_v2_request_instance = CreateDatasetsV2Request.from_json(json)
# print the JSON string representation of the object
print(CreateDatasetsV2Request.to_json())

# convert the object into a dict
create_datasets_v2_request_dict = create_datasets_v2_request_instance.to_dict()
# create an instance of CreateDatasetsV2Request from a dict
create_datasets_v2_request_from_dict = CreateDatasetsV2Request.from_dict(create_datasets_v2_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


