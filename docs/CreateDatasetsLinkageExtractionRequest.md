# CreateDatasetsLinkageExtractionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**min_id** | **int** | Minimum dataset ID to include in the term extraction | [optional] [default to 1]
**max_id** | **int** | Maximum dataset ID to include in the term extraction. Defaults to the maximum dataset ID available. | [optional] 

## Example

```python
from gateway_api_sdk.models.create_datasets_linkage_extraction_request import CreateDatasetsLinkageExtractionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateDatasetsLinkageExtractionRequest from a JSON string
create_datasets_linkage_extraction_request_instance = CreateDatasetsLinkageExtractionRequest.from_json(json)
# print the JSON string representation of the object
print(CreateDatasetsLinkageExtractionRequest.to_json())

# convert the object into a dict
create_datasets_linkage_extraction_request_dict = create_datasets_linkage_extraction_request_instance.to_dict()
# create an instance of CreateDatasetsLinkageExtractionRequest from a dict
create_datasets_linkage_extraction_request_from_dict = CreateDatasetsLinkageExtractionRequest.from_dict(create_datasets_linkage_extraction_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


