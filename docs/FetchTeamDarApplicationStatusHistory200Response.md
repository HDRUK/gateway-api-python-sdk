# FetchTeamDarApplicationStatusHistory200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**FetchTeamDarApplicationStatusHistory200ResponseData**](FetchTeamDarApplicationStatusHistory200ResponseData.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_team_dar_application_status_history200_response import FetchTeamDarApplicationStatusHistory200Response

# TODO update the JSON string below
json = "{}"
# create an instance of FetchTeamDarApplicationStatusHistory200Response from a JSON string
fetch_team_dar_application_status_history200_response_instance = FetchTeamDarApplicationStatusHistory200Response.from_json(json)
# print the JSON string representation of the object
print(FetchTeamDarApplicationStatusHistory200Response.to_json())

# convert the object into a dict
fetch_team_dar_application_status_history200_response_dict = fetch_team_dar_application_status_history200_response_instance.to_dict()
# create an instance of FetchTeamDarApplicationStatusHistory200Response from a dict
fetch_team_dar_application_status_history200_response_from_dict = FetchTeamDarApplicationStatusHistory200Response.from_dict(fetch_team_dar_application_status_history200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


