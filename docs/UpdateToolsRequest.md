# UpdateToolsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**url** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**license** | **int** |  | [optional] 
**tech_stack** | **str** |  | [optional] 
**category_id** | **int** |  | [optional] 
**user_id** | **int** |  | [optional] 
**team_id** | **int** |  | [optional] 
**tags** | **List[int]** |  | [optional] 
**dataset** | [**List[CreateToolsIntegrationsRequestDatasetInner]**](CreateToolsIntegrationsRequestDatasetInner.md) |  | [optional] 
**enabled** | **int** |  | [optional] 
**programming_language** | **List[int]** |  | [optional] 
**programming_package** | **List[int]** |  | [optional] 
**type_category** | **List[int]** |  | [optional] 
**associated_authors** | **str** |  | [optional] 
**contact_address** | **str** |  | [optional] 
**publications** | [**List[CreateToolsIntegrationsRequestPublicationsInner]**](CreateToolsIntegrationsRequestPublicationsInner.md) |  | [optional] 
**durs** | **List[int]** |  | [optional] 
**collections** | [**List[CreateToolsRequestCollectionsInner]**](CreateToolsRequestCollectionsInner.md) |  | [optional] 
**any_dataset** | **bool** |  | [optional] 
**status** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.update_tools_request import UpdateToolsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateToolsRequest from a JSON string
update_tools_request_instance = UpdateToolsRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateToolsRequest.to_json())

# convert the object into a dict
update_tools_request_dict = update_tools_request_instance.to_dict()
# create an instance of UpdateToolsRequest from a dict
update_tools_request_from_dict = UpdateToolsRequest.from_dict(update_tools_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


