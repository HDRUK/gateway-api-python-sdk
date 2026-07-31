# FetchTeamDarApplicationFiles200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**FetchTeamDarApplicationFiles200ResponseData**](FetchTeamDarApplicationFiles200ResponseData.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_team_dar_application_files200_response import FetchTeamDarApplicationFiles200Response

# TODO update the JSON string below
json = "{}"
# create an instance of FetchTeamDarApplicationFiles200Response from a JSON string
fetch_team_dar_application_files200_response_instance = FetchTeamDarApplicationFiles200Response.from_json(json)
# print the JSON string representation of the object
print(FetchTeamDarApplicationFiles200Response.to_json())

# convert the object into a dict
fetch_team_dar_application_files200_response_dict = fetch_team_dar_application_files200_response_instance.to_dict()
# create an instance of FetchTeamDarApplicationFiles200Response from a dict
fetch_team_dar_application_files200_response_from_dict = FetchTeamDarApplicationFiles200Response.from_dict(fetch_team_dar_application_files200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


