# CreateToolsIntegrationsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**url** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**license** | **str** |  | [optional] 
**tech_stack** | **str** |  | [optional] 
**category_id** | **int** |  | [optional] 
**user_id** | **int** |  | [optional] 
**team_id** | **int** |  | [optional] 
**tags** | **List[int]** |  | [optional] 
**programming_language** | **List[int]** |  | [optional] 
**programming_package** | **List[int]** |  | [optional] 
**dataset** | [**List[CreateToolsIntegrationsRequestDatasetInner]**](CreateToolsIntegrationsRequestDatasetInner.md) |  | [optional] 
**type_category** | **List[int]** |  | [optional] 
**enabled** | **int** |  | [optional] 
**publications** | [**List[CreateToolsIntegrationsRequestPublicationsInner]**](CreateToolsIntegrationsRequestPublicationsInner.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_tools_integrations_request import CreateToolsIntegrationsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateToolsIntegrationsRequest from a JSON string
create_tools_integrations_request_instance = CreateToolsIntegrationsRequest.from_json(json)
# print the JSON string representation of the object
print(CreateToolsIntegrationsRequest.to_json())

# convert the object into a dict
create_tools_integrations_request_dict = create_tools_integrations_request_instance.to_dict()
# create an instance of CreateToolsIntegrationsRequest from a dict
create_tools_integrations_request_from_dict = CreateToolsIntegrationsRequest.from_dict(create_tools_integrations_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


