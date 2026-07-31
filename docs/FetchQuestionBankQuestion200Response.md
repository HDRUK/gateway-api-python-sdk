# FetchQuestionBankQuestion200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**FetchQuestionBankQuestion200ResponseData**](FetchQuestionBankQuestion200ResponseData.md) |  | [optional] 
**version_id** | **int** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_question_bank_question200_response import FetchQuestionBankQuestion200Response

# TODO update the JSON string below
json = "{}"
# create an instance of FetchQuestionBankQuestion200Response from a JSON string
fetch_question_bank_question200_response_instance = FetchQuestionBankQuestion200Response.from_json(json)
# print the JSON string representation of the object
print(FetchQuestionBankQuestion200Response.to_json())

# convert the object into a dict
fetch_question_bank_question200_response_dict = fetch_question_bank_question200_response_instance.to_dict()
# create an instance of FetchQuestionBankQuestion200Response from a dict
fetch_question_bank_question200_response_from_dict = FetchQuestionBankQuestion200Response.from_dict(fetch_question_bank_question200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


