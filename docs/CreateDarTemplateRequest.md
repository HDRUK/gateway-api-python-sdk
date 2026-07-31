# CreateDarTemplateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**team_id** | **int** |  | 
**user_id** | **int** |  | [optional] 
**published** | **bool** |  | [optional] 
**locked** | **bool** |  | [optional] 
**questions** | [**List[CreateDarTemplateRequestQuestionsInner]**](CreateDarTemplateRequestQuestionsInner.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_dar_template_request import CreateDarTemplateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateDarTemplateRequest from a JSON string
create_dar_template_request_instance = CreateDarTemplateRequest.from_json(json)
# print the JSON string representation of the object
print(CreateDarTemplateRequest.to_json())

# convert the object into a dict
create_dar_template_request_dict = create_dar_template_request_instance.to_dict()
# create an instance of CreateDarTemplateRequest from a dict
create_dar_template_request_from_dict = CreateDarTemplateRequest.from_dict(create_dar_template_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


