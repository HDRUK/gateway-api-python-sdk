# Ada26698c9cdc86c01aaf53b0677a48d200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**current_page** | **int** |  | [optional] 
**data** | [**List[Ada26698c9cdc86c01aaf53b0677a48d200ResponseDataInner]**](Ada26698c9cdc86c01aaf53b0677a48d200ResponseDataInner.md) |  | [optional] 
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
from gateway_api_sdk.models.ada26698c9cdc86c01aaf53b0677a48d200_response import Ada26698c9cdc86c01aaf53b0677a48d200Response

# TODO update the JSON string below
json = "{}"
# create an instance of Ada26698c9cdc86c01aaf53b0677a48d200Response from a JSON string
ada26698c9cdc86c01aaf53b0677a48d200_response_instance = Ada26698c9cdc86c01aaf53b0677a48d200Response.from_json(json)
# print the JSON string representation of the object
print(Ada26698c9cdc86c01aaf53b0677a48d200Response.to_json())

# convert the object into a dict
ada26698c9cdc86c01aaf53b0677a48d200_response_dict = ada26698c9cdc86c01aaf53b0677a48d200_response_instance.to_dict()
# create an instance of Ada26698c9cdc86c01aaf53b0677a48d200Response from a dict
ada26698c9cdc86c01aaf53b0677a48d200_response_from_dict = Ada26698c9cdc86c01aaf53b0677a48d200Response.from_dict(ada26698c9cdc86c01aaf53b0677a48d200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


