# UpdatePublicationsRequest


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
**status** | **str** |  | [optional] 
**datasets** | [**List[CreatePublicationsRequestDatasetsInner]**](CreatePublicationsRequestDatasetsInner.md) |  | [optional] 
**tools** | [**List[CreatePublicationsRequestToolsInner]**](CreatePublicationsRequestToolsInner.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.update_publications_request import UpdatePublicationsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdatePublicationsRequest from a JSON string
update_publications_request_instance = UpdatePublicationsRequest.from_json(json)
# print the JSON string representation of the object
print(UpdatePublicationsRequest.to_json())

# convert the object into a dict
update_publications_request_dict = update_publications_request_instance.to_dict()
# create an instance of UpdatePublicationsRequest from a dict
update_publications_request_from_dict = UpdatePublicationsRequest.from_dict(update_publications_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


