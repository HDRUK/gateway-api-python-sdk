# FetchTeamDarApplicationHeader200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**FetchTeamDarApplicationHeader200ResponseData**](FetchTeamDarApplicationHeader200ResponseData.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_team_dar_application_header200_response import FetchTeamDarApplicationHeader200Response

# TODO update the JSON string below
json = "{}"
# create an instance of FetchTeamDarApplicationHeader200Response from a JSON string
fetch_team_dar_application_header200_response_instance = FetchTeamDarApplicationHeader200Response.from_json(json)
# print the JSON string representation of the object
print(FetchTeamDarApplicationHeader200Response.to_json())

# convert the object into a dict
fetch_team_dar_application_header200_response_dict = fetch_team_dar_application_header200_response_instance.to_dict()
# create an instance of FetchTeamDarApplicationHeader200Response from a dict
fetch_team_dar_application_header200_response_from_dict = FetchTeamDarApplicationHeader200Response.from_dict(fetch_team_dar_application_header200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


