# GetFederationByFederationIdAndTeamId200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**GetFederationByFederationIdAndTeamId200ResponseData**](GetFederationByFederationIdAndTeamId200ResponseData.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.get_federation_by_federation_id_and_team_id200_response import GetFederationByFederationIdAndTeamId200Response

# TODO update the JSON string below
json = "{}"
# create an instance of GetFederationByFederationIdAndTeamId200Response from a JSON string
get_federation_by_federation_id_and_team_id200_response_instance = GetFederationByFederationIdAndTeamId200Response.from_json(json)
# print the JSON string representation of the object
print(GetFederationByFederationIdAndTeamId200Response.to_json())

# convert the object into a dict
get_federation_by_federation_id_and_team_id200_response_dict = get_federation_by_federation_id_and_team_id200_response_instance.to_dict()
# create an instance of GetFederationByFederationIdAndTeamId200Response from a dict
get_federation_by_federation_id_and_team_id200_response_from_dict = GetFederationByFederationIdAndTeamId200Response.from_dict(get_federation_by_federation_id_and_team_id200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


