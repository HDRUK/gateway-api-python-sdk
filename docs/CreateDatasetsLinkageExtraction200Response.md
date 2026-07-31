# CreateDatasetsLinkageExtraction200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**dataset_ids** | **List[int]** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_datasets_linkage_extraction200_response import CreateDatasetsLinkageExtraction200Response

# TODO update the JSON string below
json = "{}"
# create an instance of CreateDatasetsLinkageExtraction200Response from a JSON string
create_datasets_linkage_extraction200_response_instance = CreateDatasetsLinkageExtraction200Response.from_json(json)
# print the JSON string representation of the object
print(CreateDatasetsLinkageExtraction200Response.to_json())

# convert the object into a dict
create_datasets_linkage_extraction200_response_dict = create_datasets_linkage_extraction200_response_instance.to_dict()
# create an instance of CreateDatasetsLinkageExtraction200Response from a dict
create_datasets_linkage_extraction200_response_from_dict = CreateDatasetsLinkageExtraction200Response.from_dict(create_datasets_linkage_extraction200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


