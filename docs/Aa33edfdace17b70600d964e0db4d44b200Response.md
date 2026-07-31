# Aa33edfdace17b70600d964e0db4d44b200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**current_page** | **int** |  | [optional] 
**data** | [**List[Aa33edfdace17b70600d964e0db4d44b200ResponseDataInner]**](Aa33edfdace17b70600d964e0db4d44b200ResponseDataInner.md) |  | [optional] 
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
from gateway_api_sdk.models.aa33edfdace17b70600d964e0db4d44b200_response import Aa33edfdace17b70600d964e0db4d44b200Response

# TODO update the JSON string below
json = "{}"
# create an instance of Aa33edfdace17b70600d964e0db4d44b200Response from a JSON string
aa33edfdace17b70600d964e0db4d44b200_response_instance = Aa33edfdace17b70600d964e0db4d44b200Response.from_json(json)
# print the JSON string representation of the object
print(Aa33edfdace17b70600d964e0db4d44b200Response.to_json())

# convert the object into a dict
aa33edfdace17b70600d964e0db4d44b200_response_dict = aa33edfdace17b70600d964e0db4d44b200_response_instance.to_dict()
# create an instance of Aa33edfdace17b70600d964e0db4d44b200Response from a dict
aa33edfdace17b70600d964e0db4d44b200_response_from_dict = Aa33edfdace17b70600d964e0db4d44b200Response.from_dict(aa33edfdace17b70600d964e0db4d44b200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


