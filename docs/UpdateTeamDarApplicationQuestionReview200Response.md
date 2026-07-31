# UpdateTeamDarApplicationQuestionReview200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**DataAccessApplicationReview**](DataAccessApplicationReview.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.update_team_dar_application_question_review200_response import UpdateTeamDarApplicationQuestionReview200Response

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateTeamDarApplicationQuestionReview200Response from a JSON string
update_team_dar_application_question_review200_response_instance = UpdateTeamDarApplicationQuestionReview200Response.from_json(json)
# print the JSON string representation of the object
print(UpdateTeamDarApplicationQuestionReview200Response.to_json())

# convert the object into a dict
update_team_dar_application_question_review200_response_dict = update_team_dar_application_question_review200_response_instance.to_dict()
# create an instance of UpdateTeamDarApplicationQuestionReview200Response from a dict
update_team_dar_application_question_review200_response_from_dict = UpdateTeamDarApplicationQuestionReview200Response.from_dict(update_team_dar_application_question_review200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


