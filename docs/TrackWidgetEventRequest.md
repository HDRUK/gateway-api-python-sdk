# TrackWidgetEventRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**event_type** | **str** |  | 
**entity_id** | **int** |  | [optional] 
**entity_type** | **str** |  | [optional] 
**source_domain** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.track_widget_event_request import TrackWidgetEventRequest

# TODO update the JSON string below
json = "{}"
# create an instance of TrackWidgetEventRequest from a JSON string
track_widget_event_request_instance = TrackWidgetEventRequest.from_json(json)
# print the JSON string representation of the object
print(TrackWidgetEventRequest.to_json())

# convert the object into a dict
track_widget_event_request_dict = track_widget_event_request_instance.to_dict()
# create an instance of TrackWidgetEventRequest from a dict
track_widget_event_request_from_dict = TrackWidgetEventRequest.from_dict(track_widget_event_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


