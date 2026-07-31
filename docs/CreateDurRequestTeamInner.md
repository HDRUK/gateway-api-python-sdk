# CreateDurRequestTeamInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**name** | **str** |  | [optional] 
**team_logo** | **str** |  | [optional] 
**member_of** | **str** |  | [optional] 
**contact_point** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_dur_request_team_inner import CreateDurRequestTeamInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateDurRequestTeamInner from a JSON string
create_dur_request_team_inner_instance = CreateDurRequestTeamInner.from_json(json)
# print the JSON string representation of the object
print(CreateDurRequestTeamInner.to_json())

# convert the object into a dict
create_dur_request_team_inner_dict = create_dur_request_team_inner_instance.to_dict()
# create an instance of CreateDurRequestTeamInner from a dict
create_dur_request_team_inner_from_dict = CreateDurRequestTeamInner.from_dict(create_dur_request_team_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


