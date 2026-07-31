# UpdateDarTemplateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**team_id** | **int** |  | 
**user_id** | **int** |  | [optional] 
**published** | **bool** |  | [optional] 
**locked** | **bool** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.update_dar_template_request import UpdateDarTemplateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateDarTemplateRequest from a JSON string
update_dar_template_request_instance = UpdateDarTemplateRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateDarTemplateRequest.to_json())

# convert the object into a dict
update_dar_template_request_dict = update_dar_template_request_instance.to_dict()
# create an instance of UpdateDarTemplateRequest from a dict
update_dar_template_request_from_dict = UpdateDarTemplateRequest.from_dict(update_dar_template_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


