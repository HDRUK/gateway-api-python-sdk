# Dur

A Data Use Register (DUR) entry describing an approved use of one or more datasets

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**project_title** | **str** |  | [optional] 
**project_id_text** | **str** |  | [optional] 
**organisation_name** | **str** |  | [optional] 
**organisation_sector** | **str** |  | [optional] 
**sector_id** | **int** |  | [optional] 
**lay_summary** | **str** |  | [optional] 
**technical_summary** | **str** |  | [optional] 
**latest_approval_date** | **date** |  | [optional] 
**manual_upload** | **bool** |  | [optional] 
**rejection_reason** | **str** |  | [optional] 
**sublicence_arrangements** | **str** |  | [optional] 
**public_benefit_statement** | **str** |  | [optional] 
**data_sensitivity_level** | **str** |  | [optional] 
**project_start_date** | **date** |  | [optional] 
**project_end_date** | **date** |  | [optional] 
**access_date** | **date** |  | [optional] 
**accredited_researcher_status** | **str** |  | [optional] 
**confidential_data_description** | **str** |  | [optional] 
**dataset_linkage_description** | **str** |  | [optional] 
**duty_of_confidentiality** | **str** |  | [optional] 
**legal_basis_for_data_article6** | **str** |  | [optional] 
**legal_basis_for_data_article9** | **str** |  | [optional] 
**national_data_optout** | **str** |  | [optional] 
**organisation_id** | **str** |  | [optional] 
**privacy_enhancements** | **str** |  | [optional] 
**request_category_type** | **str** |  | [optional] 
**request_frequency** | **str** |  | [optional] 
**access_type** | **str** |  | [optional] 
**non_gateway_datasets** | **List[str]** |  | [optional] 
**non_gateway_applicants** | **List[str]** |  | [optional] 
**funders_and_sponsors** | **List[str]** |  | [optional] 
**other_approval_committees** | **List[str]** |  | [optional] 
**gateway_outputs_tools** | **List[str]** |  | [optional] 
**gateway_outputs_papers** | **List[str]** |  | [optional] 
**non_gateway_outputs** | **List[str]** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**last_activity** | **datetime** |  | [optional] 
**counter** | **int** |  | [optional] 
**user_id** | **int** |  | [optional] 
**team_id** | **int** |  | [optional] 
**applicant_id** | **int** |  | [optional] 
**status** | **str** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.dur import Dur

# TODO update the JSON string below
json = "{}"
# create an instance of Dur from a JSON string
dur_instance = Dur.from_json(json)
# print the JSON string representation of the object
print(Dur.to_json())

# convert the object into a dict
dur_dict = dur_instance.to_dict()
# create an instance of Dur from a dict
dur_from_dict = Dur.from_dict(dur_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


