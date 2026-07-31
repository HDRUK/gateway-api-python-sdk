# CreateDarTemplateRequestQuestionsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**guidance** | **str** |  | [optional] 
**required** | **bool** |  | [optional] 
**order** | **int** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_dar_template_request_questions_inner import CreateDarTemplateRequestQuestionsInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateDarTemplateRequestQuestionsInner from a JSON string
create_dar_template_request_questions_inner_instance = CreateDarTemplateRequestQuestionsInner.from_json(json)
# print the JSON string representation of the object
print(CreateDarTemplateRequestQuestionsInner.to_json())

# convert the object into a dict
create_dar_template_request_questions_inner_dict = create_dar_template_request_questions_inner_instance.to_dict()
# create an instance of CreateDarTemplateRequestQuestionsInner from a dict
create_dar_template_request_questions_inner_from_dict = CreateDarTemplateRequestQuestionsInner.from_dict(create_dar_template_request_questions_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


