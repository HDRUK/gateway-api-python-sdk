# Publication

A research publication linked to one or more datasets in the Gateway

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**paper_title** | **str** |  | [optional] 
**authors** | **str** |  | [optional] 
**year_of_publication** | **int** |  | [optional] 
**paper_doi** | **str** |  | [optional] 
**publication_type** | **str** |  | [optional] 
**journal_name** | **str** |  | [optional] 
**abstract** | **str** |  | [optional] 
**url** | **str** |  | [optional] 
**owner_id** | **int** |  | [optional] 
**team_id** | **int** |  | [optional] 
**first_publication_date** | **date** |  | [optional] 
**status** | **str** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.publication import Publication

# TODO update the JSON string below
json = "{}"
# create an instance of Publication from a JSON string
publication_instance = Publication.from_json(json)
# print the JSON string representation of the object
print(Publication.to_json())

# convert the object into a dict
publication_dict = publication_instance.to_dict()
# create an instance of Publication from a dict
publication_from_dict = Publication.from_dict(publication_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


