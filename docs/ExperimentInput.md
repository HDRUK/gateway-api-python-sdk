# ExperimentInput


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**status** | **str** |  | 
**definition** | **object** | See Experiment.definition | 
**targeting** | **object** | See Experiment.targeting | 
**trigger** | **object** | See Experiment.trigger | 
**starts_at** | **date** |  | [optional] 
**ends_at** | **date** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.experiment_input import ExperimentInput

# TODO update the JSON string below
json = "{}"
# create an instance of ExperimentInput from a JSON string
experiment_input_instance = ExperimentInput.from_json(json)
# print the JSON string representation of the object
print(ExperimentInput.to_json())

# convert the object into a dict
experiment_input_dict = experiment_input_instance.to_dict()
# create an instance of ExperimentInput from a dict
experiment_input_from_dict = ExperimentInput.from_dict(experiment_input_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


