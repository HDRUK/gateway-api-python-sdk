# CreateDatasetsTermExtractionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**partial** | **bool** | Flag to determine if term extraction should be partial (true) or full (false) | [optional] [default to True]
**min_id** | **int** | Minimum dataset ID to include in the term extraction | [optional] [default to 1]
**max_id** | **int** | Maximum dataset ID to include in the term extraction. Defaults to the maximum dataset ID available. | [optional] 
**index_elastic** | **bool** | Flag to determine if data should be indexed in Elasticsearch | [optional] [default to True]

## Example

```python
from gateway_api_sdk.models.create_datasets_term_extraction_request import CreateDatasetsTermExtractionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateDatasetsTermExtractionRequest from a JSON string
create_datasets_term_extraction_request_instance = CreateDatasetsTermExtractionRequest.from_json(json)
# print the JSON string representation of the object
print(CreateDatasetsTermExtractionRequest.to_json())

# convert the object into a dict
create_datasets_term_extraction_request_dict = create_datasets_term_extraction_request_instance.to_dict()
# create an instance of CreateDatasetsTermExtractionRequest from a dict
create_datasets_term_extraction_request_from_dict = CreateDatasetsTermExtractionRequest.from_dict(create_datasets_term_extraction_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


