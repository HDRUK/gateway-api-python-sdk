# FetchTeamDarApplicationHeader200ResponseDataDatasetsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**dar_application_id** | **int** |  | [optional] 
**dataset_id** | **int** |  | [optional] 
**dataset_title** | **str** |  | [optional] 
**custodian** | [**List[FetchTeamDarApplicationHeader200ResponseDataDatasetsInnerCustodianInner]**](FetchTeamDarApplicationHeader200ResponseDataDatasetsInnerCustodianInner.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_team_dar_application_header200_response_data_datasets_inner import FetchTeamDarApplicationHeader200ResponseDataDatasetsInner

# TODO update the JSON string below
json = "{}"
# create an instance of FetchTeamDarApplicationHeader200ResponseDataDatasetsInner from a JSON string
fetch_team_dar_application_header200_response_data_datasets_inner_instance = FetchTeamDarApplicationHeader200ResponseDataDatasetsInner.from_json(json)
# print the JSON string representation of the object
print(FetchTeamDarApplicationHeader200ResponseDataDatasetsInner.to_json())

# convert the object into a dict
fetch_team_dar_application_header200_response_data_datasets_inner_dict = fetch_team_dar_application_header200_response_data_datasets_inner_instance.to_dict()
# create an instance of FetchTeamDarApplicationHeader200ResponseDataDatasetsInner from a dict
fetch_team_dar_application_header200_response_data_datasets_inner_from_dict = FetchTeamDarApplicationHeader200ResponseDataDatasetsInner.from_dict(fetch_team_dar_application_header200_response_data_datasets_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


