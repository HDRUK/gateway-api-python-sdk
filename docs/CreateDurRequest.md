# CreateDurRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**non_gateway_datasets** | **List[str]** |  | [optional] 
**non_gateway_applicants** | **List[str]** |  | [optional] 
**funders_and_sponsors** | **List[str]** |  | [optional] 
**other_approval_committees** | **List[str]** |  | [optional] 
**gateway_outputs_tools** | **List[str]** |  | [optional] 
**gateway_outputs_papers** | **List[str]** |  | [optional] 
**non_gateway_outputs** | **List[str]** |  | [optional] 
**project_title** | **str** |  | [optional] 
**project_id_text** | **str** |  | [optional] 
**organisation_name** | **str** |  | [optional] 
**organisation_sector** | **str** |  | [optional] 
**lay_summary** | **str** |  | [optional] 
**technical_summary** | **str** |  | [optional] 
**latest_approval_date** | **datetime** |  | [optional] 
**manual_upload** | **bool** |  | [optional] 
**rejection_reason** | **str** |  | [optional] 
**sublicence_arrangements** | **str** |  | [optional] 
**public_benefit_statement** | **str** |  | [optional] 
**data_sensitivity_level** | **str** |  | [optional] 
**project_start_date** | **datetime** |  | [optional] 
**project_end_date** | **datetime** |  | [optional] 
**access_date** | **datetime** |  | [optional] 
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
**mongo_object_dar_id** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**last_activity** | **datetime** |  | [optional] 
**counter** | **int** |  | [optional] 
**mongo_object_id** | **str** |  | [optional] 
**mongo_id** | **str** |  | [optional] 
**datasets** | [**List[CreateDurRequestDatasetsInner]**](CreateDurRequestDatasetsInner.md) |  | [optional] 
**publications** | [**List[CreateDurRequestPublicationsInner]**](CreateDurRequestPublicationsInner.md) |  | [optional] 
**keywords** | **List[str]** |  | [optional] 
**users** | [**List[CreateDurRequestUsersInner]**](CreateDurRequestUsersInner.md) |  | [optional] 
**user** | [**List[CreateDurRequestUsersInner]**](CreateDurRequestUsersInner.md) |  | [optional] 
**team** | [**List[CreateDurRequestTeamInner]**](CreateDurRequestTeamInner.md) |  | [optional] 
**applicant_id** | **str** |  | [optional] 
**status** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_dur_request import CreateDurRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateDurRequest from a JSON string
create_dur_request_instance = CreateDurRequest.from_json(json)
# print the JSON string representation of the object
print(CreateDurRequest.to_json())

# convert the object into a dict
create_dur_request_dict = create_dur_request_instance.to_dict()
# create an instance of CreateDurRequest from a dict
create_dur_request_from_dict = CreateDurRequest.from_dict(create_dur_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


