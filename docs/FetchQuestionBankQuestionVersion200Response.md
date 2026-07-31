# FetchQuestionBankQuestionVersion200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**FetchQuestionBankQuestionVersion200ResponseData**](FetchQuestionBankQuestionVersion200ResponseData.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_question_bank_question_version200_response import FetchQuestionBankQuestionVersion200Response

# TODO update the JSON string below
json = "{}"
# create an instance of FetchQuestionBankQuestionVersion200Response from a JSON string
fetch_question_bank_question_version200_response_instance = FetchQuestionBankQuestionVersion200Response.from_json(json)
# print the JSON string representation of the object
print(FetchQuestionBankQuestionVersion200Response.to_json())

# convert the object into a dict
fetch_question_bank_question_version200_response_dict = fetch_question_bank_question_version200_response_instance.to_dict()
# create an instance of FetchQuestionBankQuestionVersion200Response from a dict
fetch_question_bank_question_version200_response_from_dict = FetchQuestionBankQuestionVersion200Response.from_dict(fetch_question_bank_question_version200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


