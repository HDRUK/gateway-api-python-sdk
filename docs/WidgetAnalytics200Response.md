# WidgetAnalytics200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**by_event** | **List[object]** |  | [optional] 
**by_widget** | **List[object]** |  | [optional] 
**over_time** | **List[object]** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.widget_analytics200_response import WidgetAnalytics200Response

# TODO update the JSON string below
json = "{}"
# create an instance of WidgetAnalytics200Response from a JSON string
widget_analytics200_response_instance = WidgetAnalytics200Response.from_json(json)
# print the JSON string representation of the object
print(WidgetAnalytics200Response.to_json())

# convert the object into a dict
widget_analytics200_response_dict = widget_analytics200_response_instance.to_dict()
# create an instance of WidgetAnalytics200Response from a dict
widget_analytics200_response_from_dict = WidgetAnalytics200Response.from_dict(widget_analytics200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


