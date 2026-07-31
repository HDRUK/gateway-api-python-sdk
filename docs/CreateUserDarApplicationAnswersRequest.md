# CreateUserDarApplicationAnswersRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**answers** | [**List[UpdateUserDarApplicationRequestAnswersInner]**](UpdateUserDarApplicationRequestAnswersInner.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_user_dar_application_answers_request import CreateUserDarApplicationAnswersRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateUserDarApplicationAnswersRequest from a JSON string
create_user_dar_application_answers_request_instance = CreateUserDarApplicationAnswersRequest.from_json(json)
# print the JSON string representation of the object
print(CreateUserDarApplicationAnswersRequest.to_json())

# convert the object into a dict
create_user_dar_application_answers_request_dict = create_user_dar_application_answers_request_instance.to_dict()
# create an instance of CreateUserDarApplicationAnswersRequest from a dict
create_user_dar_application_answers_request_from_dict = CreateUserDarApplicationAnswersRequest.from_dict(create_user_dar_application_answers_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


