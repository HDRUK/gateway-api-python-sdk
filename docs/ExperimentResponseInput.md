# ExperimentResponseInput


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**answers** | **object** | Answers keyed by question block id; unknown ids are dropped | 
**path** | **str** |  | 
**variant** | **str** |  | [optional] 
**contact** | **bool** |  | [optional] 
**email** | **str** | Required when contact is true and not signed in | [optional] 
**recaptcha** | **str** | reCAPTCHA v3 token for the experiment_response action | 

## Example

```python
from gateway_api_sdk.models.experiment_response_input import ExperimentResponseInput

# TODO update the JSON string below
json = "{}"
# create an instance of ExperimentResponseInput from a JSON string
experiment_response_input_instance = ExperimentResponseInput.from_json(json)
# print the JSON string representation of the object
print(ExperimentResponseInput.to_json())

# convert the object into a dict
experiment_response_input_dict = experiment_response_input_instance.to_dict()
# create an instance of ExperimentResponseInput from a dict
experiment_response_input_from_dict = ExperimentResponseInput.from_dict(experiment_response_input_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


