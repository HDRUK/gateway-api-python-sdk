# FetchTeamQuestionBankQuestionsBySection200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**List[FetchTeamQuestionBankQuestionsBySection200ResponseDataInner]**](FetchTeamQuestionBankQuestionsBySection200ResponseDataInner.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_team_question_bank_questions_by_section200_response import FetchTeamQuestionBankQuestionsBySection200Response

# TODO update the JSON string below
json = "{}"
# create an instance of FetchTeamQuestionBankQuestionsBySection200Response from a JSON string
fetch_team_question_bank_questions_by_section200_response_instance = FetchTeamQuestionBankQuestionsBySection200Response.from_json(json)
# print the JSON string representation of the object
print(FetchTeamQuestionBankQuestionsBySection200Response.to_json())

# convert the object into a dict
fetch_team_question_bank_questions_by_section200_response_dict = fetch_team_question_bank_questions_by_section200_response_instance.to_dict()
# create an instance of FetchTeamQuestionBankQuestionsBySection200Response from a dict
fetch_team_question_bank_questions_by_section200_response_from_dict = FetchTeamQuestionBankQuestionsBySection200Response.from_dict(fetch_team_question_bank_questions_by_section200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


