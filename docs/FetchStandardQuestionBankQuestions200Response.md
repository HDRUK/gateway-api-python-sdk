# FetchStandardQuestionBankQuestions200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**current_page** | **int** |  | [optional] 
**data** | **List[object]** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_standard_question_bank_questions200_response import FetchStandardQuestionBankQuestions200Response

# TODO update the JSON string below
json = "{}"
# create an instance of FetchStandardQuestionBankQuestions200Response from a JSON string
fetch_standard_question_bank_questions200_response_instance = FetchStandardQuestionBankQuestions200Response.from_json(json)
# print the JSON string representation of the object
print(FetchStandardQuestionBankQuestions200Response.to_json())

# convert the object into a dict
fetch_standard_question_bank_questions200_response_dict = fetch_standard_question_bank_questions200_response_instance.to_dict()
# create an instance of FetchStandardQuestionBankQuestions200Response from a dict
fetch_standard_question_bank_questions200_response_from_dict = FetchStandardQuestionBankQuestions200Response.from_dict(fetch_standard_question_bank_questions200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


