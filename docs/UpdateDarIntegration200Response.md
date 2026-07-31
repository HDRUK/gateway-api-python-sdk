# UpdateDarIntegration200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**FetchAllDarIntegrations200ResponseDataInner**](FetchAllDarIntegrations200ResponseDataInner.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.update_dar_integration200_response import UpdateDarIntegration200Response

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateDarIntegration200Response from a JSON string
update_dar_integration200_response_instance = UpdateDarIntegration200Response.from_json(json)
# print the JSON string representation of the object
print(UpdateDarIntegration200Response.to_json())

# convert the object into a dict
update_dar_integration200_response_dict = update_dar_integration200_response_instance.to_dict()
# create an instance of UpdateDarIntegration200Response from a dict
update_dar_integration200_response_from_dict = UpdateDarIntegration200Response.from_dict(update_dar_integration200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


