# FetchAllCollections200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**List[Collection]**](Collection.md) |  | [optional] 
**first_page_url** | **str** |  | [optional] 
**var_from** | **int** |  | [optional] 
**last_page** | **int** |  | [optional] 
**last_page_url** | **str** |  | [optional] 
**links** | **List[List[object]]** |  | [optional] 
**next_page_url** | **str** |  | [optional] 
**path** | **str** |  | [optional] 
**per_page** | **int** |  | [optional] 
**prev_page_url** | **str** |  | [optional] 
**to** | **int** |  | [optional] 
**total** | **int** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_all_collections200_response import FetchAllCollections200Response

# TODO update the JSON string below
json = "{}"
# create an instance of FetchAllCollections200Response from a JSON string
fetch_all_collections200_response_instance = FetchAllCollections200Response.from_json(json)
# print the JSON string representation of the object
print(FetchAllCollections200Response.to_json())

# convert the object into a dict
fetch_all_collections200_response_dict = fetch_all_collections200_response_instance.to_dict()
# create an instance of FetchAllCollections200Response from a dict
fetch_all_collections200_response_from_dict = FetchAllCollections200Response.from_dict(fetch_all_collections200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


