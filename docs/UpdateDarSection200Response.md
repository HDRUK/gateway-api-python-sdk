# UpdateDarSection200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**UpdateDarSection200ResponseData**](UpdateDarSection200ResponseData.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.update_dar_section200_response import UpdateDarSection200Response

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateDarSection200Response from a JSON string
update_dar_section200_response_instance = UpdateDarSection200Response.from_json(json)
# print the JSON string representation of the object
print(UpdateDarSection200Response.to_json())

# convert the object into a dict
update_dar_section200_response_dict = update_dar_section200_response_instance.to_dict()
# create an instance of UpdateDarSection200Response from a dict
update_dar_section200_response_from_dict = UpdateDarSection200Response.from_dict(update_dar_section200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


