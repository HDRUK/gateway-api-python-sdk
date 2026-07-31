# RetrieveWidgetData200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**datasets** | **List[object]** |  | [optional] 
**data_uses** | **List[object]** |  | [optional] 
**scripts** | **List[object]** |  | [optional] 
**collections** | **List[object]** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.retrieve_widget_data200_response import RetrieveWidgetData200Response

# TODO update the JSON string below
json = "{}"
# create an instance of RetrieveWidgetData200Response from a JSON string
retrieve_widget_data200_response_instance = RetrieveWidgetData200Response.from_json(json)
# print the JSON string representation of the object
print(RetrieveWidgetData200Response.to_json())

# convert the object into a dict
retrieve_widget_data200_response_dict = retrieve_widget_data200_response_instance.to_dict()
# create an instance of RetrieveWidgetData200Response from a dict
retrieve_widget_data200_response_from_dict = RetrieveWidgetData200Response.from_dict(retrieve_widget_data200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


