# ExperimentTrigger


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**on** | **str** |  | [optional] 
**delay_seconds** | **int** |  | [optional] 
**frequency** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.experiment_trigger import ExperimentTrigger

# TODO update the JSON string below
json = "{}"
# create an instance of ExperimentTrigger from a JSON string
experiment_trigger_instance = ExperimentTrigger.from_json(json)
# print the JSON string representation of the object
print(ExperimentTrigger.to_json())

# convert the object into a dict
experiment_trigger_dict = experiment_trigger_instance.to_dict()
# create an instance of ExperimentTrigger from a dict
experiment_trigger_from_dict = ExperimentTrigger.from_dict(experiment_trigger_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


