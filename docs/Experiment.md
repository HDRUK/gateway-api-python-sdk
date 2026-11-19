# Experiment

A feedback prompt or design review shown to targeted visitors

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**name** | **str** |  | [optional] 
**status** | **str** |  | [optional] 
**definition** | [**ExperimentDefinition**](ExperimentDefinition.md) |  | [optional] 
**targeting** | [**ExperimentTargeting**](ExperimentTargeting.md) |  | [optional] 
**trigger** | [**ExperimentTrigger**](ExperimentTrigger.md) |  | [optional] 
**starts_at** | **date** |  | [optional] 
**ends_at** | **date** |  | [optional] 
**created_by** | **int** |  | [optional] 
**responses_count** | **int** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**deleted_at** | **datetime** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.experiment import Experiment

# TODO update the JSON string below
json = "{}"
# create an instance of Experiment from a JSON string
experiment_instance = Experiment.from_json(json)
# print the JSON string representation of the object
print(Experiment.to_json())

# convert the object into a dict
experiment_dict = experiment_instance.to_dict()
# create an instance of Experiment from a dict
experiment_from_dict = Experiment.from_dict(experiment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


