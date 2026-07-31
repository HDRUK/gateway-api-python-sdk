# CreatePublicationsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**paper_title** | **str** |  | [optional] 
**authors** | **str** |  | [optional] 
**year_of_publication** | **str** |  | [optional] 
**paper_doi** | **str** |  | [optional] 
**publication_type** | **str** |  | [optional] 
**journal_name** | **str** |  | [optional] 
**abstract** | **str** |  | [optional] 
**url** | **str** |  | [optional] 
**mongo_id** | **str** |  | [optional] 
**datasets** | [**List[CreatePublicationsRequestDatasetsInner]**](CreatePublicationsRequestDatasetsInner.md) |  | [optional] 
**tools** | [**List[CreatePublicationsRequestToolsInner]**](CreatePublicationsRequestToolsInner.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_publications_request import CreatePublicationsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreatePublicationsRequest from a JSON string
create_publications_request_instance = CreatePublicationsRequest.from_json(json)
# print the JSON string representation of the object
print(CreatePublicationsRequest.to_json())

# convert the object into a dict
create_publications_request_dict = create_publications_request_instance.to_dict()
# create an instance of CreatePublicationsRequest from a dict
create_publications_request_from_dict = CreatePublicationsRequest.from_dict(create_publications_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


