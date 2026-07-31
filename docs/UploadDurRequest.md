# UploadDurRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **int** |  | [optional] 
**team_id** | **int** |  | [optional] 
**project_title** | **str** |  | [optional] 
**project_id_text** | **str** |  | [optional] 
**organisation_name** | **str** |  | [optional] 
**organisation_id** | **str** |  | [optional] 
**organisation_sector** | **str** |  | [optional] 
**non_gateway_applicants** | **str** |  | [optional] 
**applicant_id** | **int** |  | [optional] 
**funders_and_sponsors** | **str** |  | [optional] 
**accredited_researcher_status** | **str** |  | [optional] 
**sublicence_arrangements** | **str** |  | [optional] 
**lay_summary** | **str** |  | [optional] 
**public_benefit_statement** | **str** |  | [optional] 
**request_category_type** | **str** |  | [optional] 
**technical_summary** | **str** |  | [optional] 
**other_approval_committees** | **str** |  | [optional] 
**project_start_date** | **str** |  | [optional] 
**project_end_date** | **str** |  | [optional] 
**latest_approval_date** | **str** |  | [optional] 
**data_sensitivity_level** | **str** |  | [optional] 
**legal_basis_for_data_article6** | **str** |  | [optional] 
**legal_basis_for_data_article9** | **str** |  | [optional] 
**duty_of_confidentiality** | **str** |  | [optional] 
**national_data_optout** | **str** |  | [optional] 
**request_frequency** | **str** |  | [optional] 
**dataset_linkage_description** | **str** |  | [optional] 
**confidential_data_description** | **str** |  | [optional] 
**access_date** | **str** |  | [optional] 
**access_type** | **str** |  | [optional] 
**privacy_enhancements** | **str** |  | [optional] 
**datasets** | [**List[CreateDurRequestDatasetsInner]**](CreateDurRequestDatasetsInner.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.upload_dur_request import UploadDurRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UploadDurRequest from a JSON string
upload_dur_request_instance = UploadDurRequest.from_json(json)
# print the JSON string representation of the object
print(UploadDurRequest.to_json())

# convert the object into a dict
upload_dur_request_dict = upload_dur_request_instance.to_dict()
# create an instance of UploadDurRequest from a dict
upload_dur_request_from_dict = UploadDurRequest.from_dict(upload_dur_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


