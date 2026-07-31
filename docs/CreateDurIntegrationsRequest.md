# CreateDurIntegrationsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**non_gateway_datasets** | **List[object]** |  | [optional] 
**non_gateway_applicants** | **List[object]** |  | [optional] 
**funders_and_sponsors** | **List[object]** |  | [optional] 
**other_approval_committees** | **List[object]** |  | [optional] 
**gateway_outputs_tools** | **List[object]** |  | [optional] 
**gateway_outputs_papers** | **List[object]** |  | [optional] 
**non_gateway_outputs** | **List[object]** |  | [optional] 
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
**datasets** | **List[object]** |  | [optional] 
**keywords** | **List[object]** |  | [optional] 
**users** | **List[object]** |  | [optional] 
**user** | **List[object]** |  | [optional] 
**team** | **List[object]** |  | [optional] 
**applicant_id** | **str** |  | [optional] 
**status** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_dur_integrations_request import CreateDurIntegrationsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateDurIntegrationsRequest from a JSON string
create_dur_integrations_request_instance = CreateDurIntegrationsRequest.from_json(json)
# print the JSON string representation of the object
print(CreateDurIntegrationsRequest.to_json())

# convert the object into a dict
create_dur_integrations_request_dict = create_dur_integrations_request_instance.to_dict()
# create an instance of CreateDurIntegrationsRequest from a dict
create_dur_integrations_request_from_dict = CreateDurIntegrationsRequest.from_dict(create_dur_integrations_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


