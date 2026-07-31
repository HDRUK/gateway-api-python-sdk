# UpdateDatasetsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**team_id** | **int** |  | [optional] 
**user_id** | **int** |  | [optional] 
**create_origin** | **str** |  | [optional] 
**metadata** | **object** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.update_datasets_request import UpdateDatasetsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateDatasetsRequest from a JSON string
update_datasets_request_instance = UpdateDatasetsRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateDatasetsRequest.to_json())

# convert the object into a dict
update_datasets_request_dict = update_datasets_request_instance.to_dict()
# create an instance of UpdateDatasetsRequest from a dict
update_datasets_request_from_dict = UpdateDatasetsRequest.from_dict(update_datasets_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


