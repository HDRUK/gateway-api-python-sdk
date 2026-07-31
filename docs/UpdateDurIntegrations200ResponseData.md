# UpdateDurIntegrations200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**deleted_at** | **datetime** |  | [optional] 
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
**applications** | **List[object]** |  | [optional] 
**user** | **List[object]** |  | [optional] 
**team** | **List[object]** |  | [optional] 
**application** | **List[object]** |  | [optional] 
**applicant_id** | **str** |  | [optional] 
**status** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.update_dur_integrations200_response_data import UpdateDurIntegrations200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateDurIntegrations200ResponseData from a JSON string
update_dur_integrations200_response_data_instance = UpdateDurIntegrations200ResponseData.from_json(json)
# print the JSON string representation of the object
print(UpdateDurIntegrations200ResponseData.to_json())

# convert the object into a dict
update_dur_integrations200_response_data_dict = update_dur_integrations200_response_data_instance.to_dict()
# create an instance of UpdateDurIntegrations200ResponseData from a dict
update_dur_integrations200_response_data_from_dict = UpdateDurIntegrations200ResponseData.from_dict(update_dur_integrations200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


