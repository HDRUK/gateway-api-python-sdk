# FetchQuestionBankQuestionVersion200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**deleted_at** | **datetime** |  | [optional] 
**question_id** | **int** |  | [optional] 
**version** | **int** |  | [optional] 
**default** | **bool** |  | [optional] 
**required** | **bool** |  | [optional] 
**question_json** | **object** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_question_bank_question_version200_response_data import FetchQuestionBankQuestionVersion200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of FetchQuestionBankQuestionVersion200ResponseData from a JSON string
fetch_question_bank_question_version200_response_data_instance = FetchQuestionBankQuestionVersion200ResponseData.from_json(json)
# print the JSON string representation of the object
print(FetchQuestionBankQuestionVersion200ResponseData.to_json())

# convert the object into a dict
fetch_question_bank_question_version200_response_data_dict = fetch_question_bank_question_version200_response_data_instance.to_dict()
# create an instance of FetchQuestionBankQuestionVersion200ResponseData from a dict
fetch_question_bank_question_version200_response_data_from_dict = FetchQuestionBankQuestionVersion200ResponseData.from_dict(fetch_question_bank_question_version200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


