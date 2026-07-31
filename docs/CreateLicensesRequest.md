# CreateLicensesRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **str** |  | 
**label** | **str** |  | 
**valid_since** | **datetime** |  | 
**valid_until** | **datetime** |  | [optional] 
**definition** | **str** |  | 
**origin** | **str** |  | 

## Example

```python
from gateway_api_sdk.models.create_licenses_request import CreateLicensesRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateLicensesRequest from a JSON string
create_licenses_request_instance = CreateLicensesRequest.from_json(json)
# print the JSON string representation of the object
print(CreateLicensesRequest.to_json())

# convert the object into a dict
create_licenses_request_dict = create_licenses_request_instance.to_dict()
# create an instance of CreateLicensesRequest from a dict
create_licenses_request_from_dict = CreateLicensesRequest.from_dict(create_licenses_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


