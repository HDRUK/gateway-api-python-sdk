# ExperimentDefinition

Steps and blocks rendered by @hdruk/experiments

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**steps** | [**List[ExperimentDefinitionStepsInner]**](ExperimentDefinitionStepsInner.md) |  | [optional] 
**thank_you** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.experiment_definition import ExperimentDefinition

# TODO update the JSON string below
json = "{}"
# create an instance of ExperimentDefinition from a JSON string
experiment_definition_instance = ExperimentDefinition.from_json(json)
# print the JSON string representation of the object
print(ExperimentDefinition.to_json())

# convert the object into a dict
experiment_definition_dict = experiment_definition_instance.to_dict()
# create an instance of ExperimentDefinition from a dict
experiment_definition_from_dict = ExperimentDefinition.from_dict(experiment_definition_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


