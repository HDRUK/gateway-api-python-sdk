# ActiveExperiment

An experiment as served to a visitor, without its targeting rules

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**name** | **str** |  | [optional] 
**paths** | **List[str]** |  | [optional] 
**trigger** | **object** | See Experiment.trigger | [optional] 
**definition** | **object** | See Experiment.definition | [optional] 
**variant** | **str** |  | [optional] 
**ends_at** | **date** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.active_experiment import ActiveExperiment

# TODO update the JSON string below
json = "{}"
# create an instance of ActiveExperiment from a JSON string
active_experiment_instance = ActiveExperiment.from_json(json)
# print the JSON string representation of the object
print(ActiveExperiment.to_json())

# convert the object into a dict
active_experiment_dict = active_experiment_instance.to_dict()
# create an instance of ActiveExperiment from a dict
active_experiment_from_dict = ActiveExperiment.from_dict(active_experiment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


