# CreateQuestionBankQuestionRequestOptionsInnerChildrenInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**force_required** | **bool** |  | [optional] 
**allow_guidance_override** | **bool** |  | [optional] 
**locked** | **bool** |  | [optional] 
**archived** | **bool** |  | [optional] 
**component** | **str** |  | [optional] 
**validations** | **List[object]** |  | [optional] 
**options** | [**List[CreateQuestionBankQuestionRequestOptionsInnerChildrenInnerOptionsInner]**](CreateQuestionBankQuestionRequestOptionsInnerChildrenInnerOptionsInner.md) |  | [optional] 
**title** | **str** |  | [optional] 
**guidance** | **str** |  | [optional] 
**required** | **bool** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_question_bank_question_request_options_inner_children_inner import CreateQuestionBankQuestionRequestOptionsInnerChildrenInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateQuestionBankQuestionRequestOptionsInnerChildrenInner from a JSON string
create_question_bank_question_request_options_inner_children_inner_instance = CreateQuestionBankQuestionRequestOptionsInnerChildrenInner.from_json(json)
# print the JSON string representation of the object
print(CreateQuestionBankQuestionRequestOptionsInnerChildrenInner.to_json())

# convert the object into a dict
create_question_bank_question_request_options_inner_children_inner_dict = create_question_bank_question_request_options_inner_children_inner_instance.to_dict()
# create an instance of CreateQuestionBankQuestionRequestOptionsInnerChildrenInner from a dict
create_question_bank_question_request_options_inner_children_inner_from_dict = CreateQuestionBankQuestionRequestOptionsInnerChildrenInner.from_dict(create_question_bank_question_request_options_inner_children_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


