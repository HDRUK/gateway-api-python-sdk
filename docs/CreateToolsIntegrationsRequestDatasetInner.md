# CreateToolsIntegrationsRequestDatasetInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**link_type** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_tools_integrations_request_dataset_inner import CreateToolsIntegrationsRequestDatasetInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateToolsIntegrationsRequestDatasetInner from a JSON string
create_tools_integrations_request_dataset_inner_instance = CreateToolsIntegrationsRequestDatasetInner.from_json(json)
# print the JSON string representation of the object
print(CreateToolsIntegrationsRequestDatasetInner.to_json())

# convert the object into a dict
create_tools_integrations_request_dataset_inner_dict = create_tools_integrations_request_dataset_inner_instance.to_dict()
# create an instance of CreateToolsIntegrationsRequestDatasetInner from a dict
create_tools_integrations_request_dataset_inner_from_dict = CreateToolsIntegrationsRequestDatasetInner.from_dict(create_tools_integrations_request_dataset_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


