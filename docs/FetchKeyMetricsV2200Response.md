# FetchKeyMetricsV2200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | **List[List[object]]** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_key_metrics_v2200_response import FetchKeyMetricsV2200Response

# TODO update the JSON string below
json = "{}"
# create an instance of FetchKeyMetricsV2200Response from a JSON string
fetch_key_metrics_v2200_response_instance = FetchKeyMetricsV2200Response.from_json(json)
# print the JSON string representation of the object
print(FetchKeyMetricsV2200Response.to_json())

# convert the object into a dict
fetch_key_metrics_v2200_response_dict = fetch_key_metrics_v2200_response_instance.to_dict()
# create an instance of FetchKeyMetricsV2200Response from a dict
fetch_key_metrics_v2200_response_from_dict = FetchKeyMetricsV2200Response.from_dict(fetch_key_metrics_v2200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


