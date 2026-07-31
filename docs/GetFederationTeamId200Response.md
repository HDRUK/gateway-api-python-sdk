# GetFederationTeamId200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**current_page** | **int** |  | [optional] 
**data** | [**List[GetFederationTeamId200ResponseDataInner]**](GetFederationTeamId200ResponseDataInner.md) |  | [optional] 
**first_page_url** | **str** |  | [optional] 
**var_from** | **int** |  | [optional] 
**last_page** | **int** |  | [optional] 
**last_page_url** | **str** |  | [optional] 
**links** | **List[List[object]]** |  | [optional] 
**next_page_url** | **str** |  | [optional] 
**path** | **str** |  | [optional] 
**per_page** | **int** |  | [optional] 
**prev_page_url** | **str** |  | [optional] 
**to** | **int** |  | [optional] 
**total** | **int** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.get_federation_team_id200_response import GetFederationTeamId200Response

# TODO update the JSON string below
json = "{}"
# create an instance of GetFederationTeamId200Response from a JSON string
get_federation_team_id200_response_instance = GetFederationTeamId200Response.from_json(json)
# print the JSON string representation of the object
print(GetFederationTeamId200Response.to_json())

# convert the object into a dict
get_federation_team_id200_response_dict = get_federation_team_id200_response_instance.to_dict()
# create an instance of GetFederationTeamId200Response from a dict
get_federation_team_id200_response_from_dict = GetFederationTeamId200Response.from_dict(get_federation_team_id200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


