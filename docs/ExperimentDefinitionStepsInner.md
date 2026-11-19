# ExperimentDefinitionStepsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**blocks** | [**List[ExperimentDefinitionStepsInnerBlocksInner]**](ExperimentDefinitionStepsInnerBlocksInner.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.experiment_definition_steps_inner import ExperimentDefinitionStepsInner

# TODO update the JSON string below
json = "{}"
# create an instance of ExperimentDefinitionStepsInner from a JSON string
experiment_definition_steps_inner_instance = ExperimentDefinitionStepsInner.from_json(json)
# print the JSON string representation of the object
print(ExperimentDefinitionStepsInner.to_json())

# convert the object into a dict
experiment_definition_steps_inner_dict = experiment_definition_steps_inner_instance.to_dict()
# create an instance of ExperimentDefinitionStepsInner from a dict
experiment_definition_steps_inner_from_dict = ExperimentDefinitionStepsInner.from_dict(experiment_definition_steps_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


