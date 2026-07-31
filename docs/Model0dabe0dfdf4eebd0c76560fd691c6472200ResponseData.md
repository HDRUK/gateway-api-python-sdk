# Model0dabe0dfdf4eebd0c76560fd691c6472200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**deleted_at** | **datetime** |  | [optional] 
**applicant_id** | **int** |  | [optional] 
**project_title** | **str** |  | [optional] 
**application_type** | **str** |  | [optional] 
**project_id** | **int** |  | [optional] 
**is_joint** | **bool** |  | [optional] 
**approval_status** | **str** |  | [optional] 
**submission_status** | **str** |  | [optional] 
**status_review_id** | **int** |  | [optional] 
**days_since_submission** | **int** |  | [optional] 
**primary_applicant** | [**List[Model0dabe0dfdf4eebd0c76560fd691c6472200ResponseDataPrimaryApplicantInner]**](Model0dabe0dfdf4eebd0c76560fd691c6472200ResponseDataPrimaryApplicantInner.md) |  | [optional] 
**datasets** | [**List[Model0dabe0dfdf4eebd0c76560fd691c6472200ResponseDataDatasetsInner]**](Model0dabe0dfdf4eebd0c76560fd691c6472200ResponseDataDatasetsInner.md) |  | [optional] 
**teams** | [**List[Model0dabe0dfdf4eebd0c76560fd691c6472200ResponseDataTeamsInner]**](Model0dabe0dfdf4eebd0c76560fd691c6472200ResponseDataTeamsInner.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.model0dabe0dfdf4eebd0c76560fd691c6472200_response_data import Model0dabe0dfdf4eebd0c76560fd691c6472200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of Model0dabe0dfdf4eebd0c76560fd691c6472200ResponseData from a JSON string
model0dabe0dfdf4eebd0c76560fd691c6472200_response_data_instance = Model0dabe0dfdf4eebd0c76560fd691c6472200ResponseData.from_json(json)
# print the JSON string representation of the object
print(Model0dabe0dfdf4eebd0c76560fd691c6472200ResponseData.to_json())

# convert the object into a dict
model0dabe0dfdf4eebd0c76560fd691c6472200_response_data_dict = model0dabe0dfdf4eebd0c76560fd691c6472200_response_data_instance.to_dict()
# create an instance of Model0dabe0dfdf4eebd0c76560fd691c6472200ResponseData from a dict
model0dabe0dfdf4eebd0c76560fd691c6472200_response_data_from_dict = Model0dabe0dfdf4eebd0c76560fd691c6472200ResponseData.from_dict(model0dabe0dfdf4eebd0c76560fd691c6472200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


