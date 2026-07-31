# UpdateUserDarApplicationRequestAnswersInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**question_id** | **int** |  | [optional] 
**answer** | [**UpdateUserDarApplicationRequestAnswersInnerAnswer**](UpdateUserDarApplicationRequestAnswersInnerAnswer.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.update_user_dar_application_request_answers_inner import UpdateUserDarApplicationRequestAnswersInner

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateUserDarApplicationRequestAnswersInner from a JSON string
update_user_dar_application_request_answers_inner_instance = UpdateUserDarApplicationRequestAnswersInner.from_json(json)
# print the JSON string representation of the object
print(UpdateUserDarApplicationRequestAnswersInner.to_json())

# convert the object into a dict
update_user_dar_application_request_answers_inner_dict = update_user_dar_application_request_answers_inner_instance.to_dict()
# create an instance of UpdateUserDarApplicationRequestAnswersInner from a dict
update_user_dar_application_request_answers_inner_from_dict = UpdateUserDarApplicationRequestAnswersInner.from_dict(update_user_dar_application_request_answers_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


