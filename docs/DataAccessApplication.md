# DataAccessApplication

A Data Access Application (DAR) record managed by the Gateway

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**applicant_id** | **int** |  | [optional] 
**project_title** | **str** |  | [optional] 
**project_id** | **str** |  | [optional] 
**application_type** | **str** |  | [optional] 
**submission_status** | **str** |  | [optional] 
**approval_status** | **str** |  | [optional] 
**is_joint** | **bool** |  | [optional] 
**status_review_id** | **int** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**deleted_at** | **datetime** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.data_access_application import DataAccessApplication

# TODO update the JSON string below
json = "{}"
# create an instance of DataAccessApplication from a JSON string
data_access_application_instance = DataAccessApplication.from_json(json)
# print the JSON string representation of the object
print(DataAccessApplication.to_json())

# convert the object into a dict
data_access_application_dict = data_access_application_instance.to_dict()
# create an instance of DataAccessApplication from a dict
data_access_application_from_dict = DataAccessApplication.from_dict(data_access_application_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


