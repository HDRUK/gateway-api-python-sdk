# CreateQuestionBankQuestionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**section_id** | **int** |  | 
**user_id** | **int** |  | [optional] 
**team_ids** | **List[int]** |  | [optional] 
**locked** | **bool** |  | [optional] 
**archived** | **bool** |  | [optional] 
**required** | **bool** |  | [optional] 
**force_required** | **bool** |  | 
**allow_guidance_override** | **bool** |  | 
**default** | **bool** |  | [optional] 
**guidance** | **str** |  | 
**title** | **str** |  | 
**var_field** | **List[object]** |  | 
**component** | **str** |  | 
**validations** | **List[object]** |  | 
**options** | [**List[CreateQuestionBankQuestionRequestOptionsInner]**](CreateQuestionBankQuestionRequestOptionsInner.md) |  | 
**is_child** | **bool** |  | [optional] 
**question_type** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_question_bank_question_request import CreateQuestionBankQuestionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateQuestionBankQuestionRequest from a JSON string
create_question_bank_question_request_instance = CreateQuestionBankQuestionRequest.from_json(json)
# print the JSON string representation of the object
print(CreateQuestionBankQuestionRequest.to_json())

# convert the object into a dict
create_question_bank_question_request_dict = create_question_bank_question_request_instance.to_dict()
# create an instance of CreateQuestionBankQuestionRequest from a dict
create_question_bank_question_request_from_dict = CreateQuestionBankQuestionRequest.from_dict(create_question_bank_question_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


