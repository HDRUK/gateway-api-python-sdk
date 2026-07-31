# Team

A data custodian team that owns datasets and manages data access

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**name** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**allows_messaging** | **bool** |  | [optional] 
**workflow_enabled** | **bool** |  | [optional] 
**access_requests_management** | **bool** |  | [optional] 
**uses_5_safes** | **bool** |  | [optional] 
**is_admin** | **bool** |  | [optional] 
**member_of** | **str** |  | [optional] 
**contact_point** | **str** |  | [optional] 
**notification_status** | **bool** |  | [optional] 
**is_question_bank** | **bool** |  | [optional] 
**team_logo** | **str** |  | [optional] 
**introduction** | **str** |  | [optional] 
**dar_modal_content** | **str** |  | [optional] 
**dar_modal_header** | **str** |  | [optional] 
**dar_modal_footer** | **str** |  | [optional] 
**service** | **str** |  | [optional] 
**is_dar** | **bool** |  | [optional] 
**pid** | **str** | Public identifier, cast to string | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.team import Team

# TODO update the JSON string below
json = "{}"
# create an instance of Team from a JSON string
team_instance = Team.from_json(json)
# print the JSON string representation of the object
print(Team.to_json())

# convert the object into a dict
team_dict = team_instance.to_dict()
# create an instance of Team from a dict
team_from_dict = Team.from_dict(team_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


