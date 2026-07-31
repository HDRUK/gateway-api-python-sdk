# CreateApplicationsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**image_link** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**team_id** | **int** |  | [optional] 
**user_id** | **int** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**permissions** | **List[object]** |  | [optional] 
**notifications** | **List[object]** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_applications_request import CreateApplicationsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateApplicationsRequest from a JSON string
create_applications_request_instance = CreateApplicationsRequest.from_json(json)
# print the JSON string representation of the object
print(CreateApplicationsRequest.to_json())

# convert the object into a dict
create_applications_request_dict = create_applications_request_instance.to_dict()
# create an instance of CreateApplicationsRequest from a dict
create_applications_request_from_dict = CreateApplicationsRequest.from_dict(create_applications_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


