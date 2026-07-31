# UpdateQuestionBankQuestionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**section_id** | **int** |  | 
**user_id** | **int** |  | [optional] 
**team_ids** | **List[int]** |  | [optional] 
**locked** | **bool** |  | [optional] 
**archived** | **bool** |  | [optional] 
**is_child** | **bool** |  | [optional] 
**question_type** | **str** |  | [optional] 
**required** | **bool** |  | [optional] 
**force_required** | **bool** |  | 
**allow_guidance_override** | **bool** |  | 
**default** | **bool** |  | [optional] 
**guidance** | **str** |  | 
**title** | **str** |  | 
**var_field** | **List[object]** |  | 

## Example

```python
from gateway_api_sdk.models.update_question_bank_question_request import UpdateQuestionBankQuestionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateQuestionBankQuestionRequest from a JSON string
update_question_bank_question_request_instance = UpdateQuestionBankQuestionRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateQuestionBankQuestionRequest.to_json())

# convert the object into a dict
update_question_bank_question_request_dict = update_question_bank_question_request_instance.to_dict()
# create an instance of UpdateQuestionBankQuestionRequest from a dict
update_question_bank_question_request_from_dict = UpdateQuestionBankQuestionRequest.from_dict(update_question_bank_question_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


