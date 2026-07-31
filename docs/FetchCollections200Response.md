# FetchCollections200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**Collection**](Collection.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_collections200_response import FetchCollections200Response

# TODO update the JSON string below
json = "{}"
# create an instance of FetchCollections200Response from a JSON string
fetch_collections200_response_instance = FetchCollections200Response.from_json(json)
# print the JSON string representation of the object
print(FetchCollections200Response.to_json())

# convert the object into a dict
fetch_collections200_response_dict = fetch_collections200_response_instance.to_dict()
# create an instance of FetchCollections200Response from a dict
fetch_collections200_response_from_dict = FetchCollections200Response.from_dict(fetch_collections200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


