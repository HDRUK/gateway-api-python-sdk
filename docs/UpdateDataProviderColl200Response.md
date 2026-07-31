# UpdateDataProviderColl200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**FetchDataProviderColls200ResponseDataInner**](FetchDataProviderColls200ResponseDataInner.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.update_data_provider_coll200_response import UpdateDataProviderColl200Response

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateDataProviderColl200Response from a JSON string
update_data_provider_coll200_response_instance = UpdateDataProviderColl200Response.from_json(json)
# print the JSON string representation of the object
print(UpdateDataProviderColl200Response.to_json())

# convert the object into a dict
update_data_provider_coll200_response_dict = update_data_provider_coll200_response_instance.to_dict()
# create an instance of UpdateDataProviderColl200Response from a dict
update_data_provider_coll200_response_from_dict = UpdateDataProviderColl200Response.from_dict(update_data_provider_coll200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


