# UpdateWidget200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**Widget**](Widget.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.update_widget200_response import UpdateWidget200Response

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateWidget200Response from a JSON string
update_widget200_response_instance = UpdateWidget200Response.from_json(json)
# print the JSON string representation of the object
print(UpdateWidget200Response.to_json())

# convert the object into a dict
update_widget200_response_dict = update_widget200_response_instance.to_dict()
# create an instance of UpdateWidget200Response from a dict
update_widget200_response_from_dict = UpdateWidget200Response.from_dict(update_widget200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


