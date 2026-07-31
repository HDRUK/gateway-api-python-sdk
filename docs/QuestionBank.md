# QuestionBank

A question bank question record managed by the Gateway

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**section_id** | **int** |  | [optional] 
**user_id** | **int** |  | [optional] 
**locked** | **bool** |  | [optional] 
**archived** | **bool** |  | [optional] 
**archived_date** | **datetime** |  | [optional] 
**force_required** | **bool** |  | [optional] 
**allow_guidance_override** | **bool** |  | [optional] 
**is_child** | **bool** |  | [optional] 
**question_type** | **str** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.question_bank import QuestionBank

# TODO update the JSON string below
json = "{}"
# create an instance of QuestionBank from a JSON string
question_bank_instance = QuestionBank.from_json(json)
# print the JSON string representation of the object
print(QuestionBank.to_json())

# convert the object into a dict
question_bank_dict = question_bank_instance.to_dict()
# create an instance of QuestionBank from a dict
question_bank_from_dict = QuestionBank.from_dict(question_bank_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


