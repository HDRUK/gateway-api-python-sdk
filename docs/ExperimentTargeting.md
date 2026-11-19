# ExperimentTargeting


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**paths** | **List[str]** |  | [optional] 
**audience** | **str** |  | [optional] 
**user_ids** | **List[int]** |  | [optional] 
**percentage** | **int** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.experiment_targeting import ExperimentTargeting

# TODO update the JSON string below
json = "{}"
# create an instance of ExperimentTargeting from a JSON string
experiment_targeting_instance = ExperimentTargeting.from_json(json)
# print the JSON string representation of the object
print(ExperimentTargeting.to_json())

# convert the object into a dict
experiment_targeting_dict = experiment_targeting_instance.to_dict()
# create an instance of ExperimentTargeting from a dict
experiment_targeting_from_dict = ExperimentTargeting.from_dict(experiment_targeting_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


