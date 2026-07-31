# CreateDarApplicationsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**applicant_id** | **int** |  | [optional] 
**submission_status** | **str** |  | [optional] 
**approval_status** | **str** |  | [optional] 
**project_title** | **str** |  | [optional] 
**team_ids** | **List[int]** |  | [optional] 
**dataset_ids** | **List[int]** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_dar_applications_request import CreateDarApplicationsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateDarApplicationsRequest from a JSON string
create_dar_applications_request_instance = CreateDarApplicationsRequest.from_json(json)
# print the JSON string representation of the object
print(CreateDarApplicationsRequest.to_json())

# convert the object into a dict
create_dar_applications_request_dict = create_dar_applications_request_instance.to_dict()
# create an instance of CreateDarApplicationsRequest from a dict
create_dar_applications_request_from_dict = CreateDarApplicationsRequest.from_dict(create_dar_applications_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


