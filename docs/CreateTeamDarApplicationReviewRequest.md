# CreateTeamDarApplicationReviewRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**comment** | **str** |  | 

## Example

```python
from gateway_api_sdk.models.create_team_dar_application_review_request import CreateTeamDarApplicationReviewRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateTeamDarApplicationReviewRequest from a JSON string
create_team_dar_application_review_request_instance = CreateTeamDarApplicationReviewRequest.from_json(json)
# print the JSON string representation of the object
print(CreateTeamDarApplicationReviewRequest.to_json())

# convert the object into a dict
create_team_dar_application_review_request_dict = create_team_dar_application_review_request_instance.to_dict()
# create an instance of CreateTeamDarApplicationReviewRequest from a dict
create_team_dar_application_review_request_from_dict = CreateTeamDarApplicationReviewRequest.from_dict(create_team_dar_application_review_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


