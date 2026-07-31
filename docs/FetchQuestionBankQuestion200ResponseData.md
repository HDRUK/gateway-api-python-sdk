# FetchQuestionBankQuestion200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**deleted_at** | **datetime** |  | [optional] 
**question_id** | **int** |  | [optional] 
**version** | **int** |  | [optional] 
**default** | **bool** |  | [optional] 
**required** | **bool** |  | [optional] 
**section_id** | **int** |  | [optional] 
**user_id** | **int** |  | [optional] 
**locked** | **bool** |  | [optional] 
**archived** | **bool** |  | [optional] 
**archived_date** | **datetime** |  | [optional] 
**force_required** | **bool** |  | [optional] 
**allow_guidance_override** | **bool** |  | [optional] 
**is_child** | **int** |  | [optional] 
**question_type** | **str** |  | [optional] 
**title** | **str** |  | [optional] 
**guidance** | **str** |  | [optional] 
**options** | **List[object]** |  | [optional] 
**component** | **str** |  | [optional] 
**validations** | **List[object]** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_question_bank_question200_response_data import FetchQuestionBankQuestion200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of FetchQuestionBankQuestion200ResponseData from a JSON string
fetch_question_bank_question200_response_data_instance = FetchQuestionBankQuestion200ResponseData.from_json(json)
# print the JSON string representation of the object
print(FetchQuestionBankQuestion200ResponseData.to_json())

# convert the object into a dict
fetch_question_bank_question200_response_data_dict = fetch_question_bank_question200_response_data_instance.to_dict()
# create an instance of FetchQuestionBankQuestion200ResponseData from a dict
fetch_question_bank_question200_response_data_from_dict = FetchQuestionBankQuestion200ResponseData.from_dict(fetch_question_bank_question200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


