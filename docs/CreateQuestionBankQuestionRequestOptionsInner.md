# CreateQuestionBankQuestionRequestOptionsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**label** | **str** |  | [optional] 
**children** | [**List[CreateQuestionBankQuestionRequestOptionsInnerChildrenInner]**](CreateQuestionBankQuestionRequestOptionsInnerChildrenInner.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_question_bank_question_request_options_inner import CreateQuestionBankQuestionRequestOptionsInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateQuestionBankQuestionRequestOptionsInner from a JSON string
create_question_bank_question_request_options_inner_instance = CreateQuestionBankQuestionRequestOptionsInner.from_json(json)
# print the JSON string representation of the object
print(CreateQuestionBankQuestionRequestOptionsInner.to_json())

# convert the object into a dict
create_question_bank_question_request_options_inner_dict = create_question_bank_question_request_options_inner_instance.to_dict()
# create an instance of CreateQuestionBankQuestionRequestOptionsInner from a dict
create_question_bank_question_request_options_inner_from_dict = CreateQuestionBankQuestionRequestOptionsInner.from_dict(create_question_bank_question_request_options_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


