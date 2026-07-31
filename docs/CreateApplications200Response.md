# CreateApplications200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**List[CreateApplications200ResponseDataInner]**](CreateApplications200ResponseDataInner.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_applications200_response import CreateApplications200Response

# TODO update the JSON string below
json = "{}"
# create an instance of CreateApplications200Response from a JSON string
create_applications200_response_instance = CreateApplications200Response.from_json(json)
# print the JSON string representation of the object
print(CreateApplications200Response.to_json())

# convert the object into a dict
create_applications200_response_dict = create_applications200_response_instance.to_dict()
# create an instance of CreateApplications200Response from a dict
create_applications200_response_from_dict = CreateApplications200Response.from_dict(create_applications200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


