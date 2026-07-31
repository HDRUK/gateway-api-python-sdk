# FetchDurByIdIntegrations200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**List[FetchDurByIdIntegrations200ResponseDataInner]**](FetchDurByIdIntegrations200ResponseDataInner.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_dur_by_id_integrations200_response import FetchDurByIdIntegrations200Response

# TODO update the JSON string below
json = "{}"
# create an instance of FetchDurByIdIntegrations200Response from a JSON string
fetch_dur_by_id_integrations200_response_instance = FetchDurByIdIntegrations200Response.from_json(json)
# print the JSON string representation of the object
print(FetchDurByIdIntegrations200Response.to_json())

# convert the object into a dict
fetch_dur_by_id_integrations200_response_dict = fetch_dur_by_id_integrations200_response_instance.to_dict()
# create an instance of FetchDurByIdIntegrations200Response from a dict
fetch_dur_by_id_integrations200_response_from_dict = FetchDurByIdIntegrations200Response.from_dict(fetch_dur_by_id_integrations200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


