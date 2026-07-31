# CreatePublicationsRequestDatasetsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**link_type** | **str** |  | [optional] 
**description** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_publications_request_datasets_inner import CreatePublicationsRequestDatasetsInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreatePublicationsRequestDatasetsInner from a JSON string
create_publications_request_datasets_inner_instance = CreatePublicationsRequestDatasetsInner.from_json(json)
# print the JSON string representation of the object
print(CreatePublicationsRequestDatasetsInner.to_json())

# convert the object into a dict
create_publications_request_datasets_inner_dict = create_publications_request_datasets_inner_instance.to_dict()
# create an instance of CreatePublicationsRequestDatasetsInner from a dict
create_publications_request_datasets_inner_from_dict = CreatePublicationsRequestDatasetsInner.from_dict(create_publications_request_datasets_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


