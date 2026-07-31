# EditQuestionBankQuestionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**section_id** | **int** |  | [optional] 
**user_id** | **int** |  | [optional] 
**team_ids** | **List[int]** |  | [optional] 
**locked** | **bool** |  | [optional] 
**archived** | **bool** |  | [optional] 
**force_required** | **bool** |  | [optional] 
**allow_guidance_override** | **bool** |  | [optional] 
**question_type** | **str** |  | [optional] 
**default** | **bool** |  | [optional] 
**guidance** | **str** |  | [optional] 
**title** | **str** |  | [optional] 
**var_field** | **List[object]** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.edit_question_bank_question_request import EditQuestionBankQuestionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EditQuestionBankQuestionRequest from a JSON string
edit_question_bank_question_request_instance = EditQuestionBankQuestionRequest.from_json(json)
# print the JSON string representation of the object
print(EditQuestionBankQuestionRequest.to_json())

# convert the object into a dict
edit_question_bank_question_request_dict = edit_question_bank_question_request_instance.to_dict()
# create an instance of EditQuestionBankQuestionRequest from a dict
edit_question_bank_question_request_from_dict = EditQuestionBankQuestionRequest.from_dict(edit_question_bank_question_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


