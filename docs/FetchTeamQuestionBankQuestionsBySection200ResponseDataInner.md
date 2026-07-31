# FetchTeamQuestionBankQuestionsBySection200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**deleted_at** | **datetime** |  | [optional] 
**section_id** | **int** |  | [optional] 
**user_id** | **int** |  | [optional] 
**locked** | **bool** |  | [optional] 
**archived** | **bool** |  | [optional] 
**archived_date** | **datetime** |  | [optional] 
**force_required** | **bool** |  | [optional] 
**allow_guidance_override** | **bool** |  | [optional] 
**is_child** | **bool** |  | [optional] 
**question_type** | **str** |  | [optional] 
**latest_version** | **object** |  | [optional] 
**versions** | **object** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_team_question_bank_questions_by_section200_response_data_inner import FetchTeamQuestionBankQuestionsBySection200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of FetchTeamQuestionBankQuestionsBySection200ResponseDataInner from a JSON string
fetch_team_question_bank_questions_by_section200_response_data_inner_instance = FetchTeamQuestionBankQuestionsBySection200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(FetchTeamQuestionBankQuestionsBySection200ResponseDataInner.to_json())

# convert the object into a dict
fetch_team_question_bank_questions_by_section200_response_data_inner_dict = fetch_team_question_bank_questions_by_section200_response_data_inner_instance.to_dict()
# create an instance of FetchTeamQuestionBankQuestionsBySection200ResponseDataInner from a dict
fetch_team_question_bank_questions_by_section200_response_data_inner_from_dict = FetchTeamQuestionBankQuestionsBySection200ResponseDataInner.from_dict(fetch_team_question_bank_questions_by_section200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


