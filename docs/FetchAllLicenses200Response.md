# FetchAllLicenses200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**current_page** | **int** |  | [optional] 
**data** | [**List[License]**](License.md) |  | [optional] 
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
from gateway_api_sdk.models.fetch_all_licenses200_response import FetchAllLicenses200Response

# TODO update the JSON string below
json = "{}"
# create an instance of FetchAllLicenses200Response from a JSON string
fetch_all_licenses200_response_instance = FetchAllLicenses200Response.from_json(json)
# print the JSON string representation of the object
print(FetchAllLicenses200Response.to_json())

# convert the object into a dict
fetch_all_licenses200_response_dict = fetch_all_licenses200_response_instance.to_dict()
# create an instance of FetchAllLicenses200Response from a dict
fetch_all_licenses200_response_from_dict = FetchAllLicenses200Response.from_dict(fetch_all_licenses200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


