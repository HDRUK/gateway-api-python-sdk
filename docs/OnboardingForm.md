# OnboardingForm

The data the metadata onboarding form is generated from

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**schemas** | [**List[OnboardingFormSchemasInner]**](OnboardingFormSchemasInner.md) |  | [optional] 
**model** | **str** |  | [optional] 
**version** | **str** |  | [optional] 
**var_schema** | **object** | JSON Schema of the selected input schema | [optional] 
**default_values** | **object** | Team defaults in the selected schema | [optional] 
**metadata** | **object** | Only with dataset_id | [optional] 

## Example

```python
from gateway_api_sdk.models.onboarding_form import OnboardingForm

# TODO update the JSON string below
json = "{}"
# create an instance of OnboardingForm from a JSON string
onboarding_form_instance = OnboardingForm.from_json(json)
# print the JSON string representation of the object
print(OnboardingForm.to_json())

# convert the object into a dict
onboarding_form_dict = onboarding_form_instance.to_dict()
# create an instance of OnboardingForm from a dict
onboarding_form_from_dict = OnboardingForm.from_dict(onboarding_form_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


