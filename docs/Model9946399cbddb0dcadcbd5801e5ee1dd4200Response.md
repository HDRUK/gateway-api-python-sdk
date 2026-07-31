# Model9946399cbddb0dcadcbd5801e5ee1dd4200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**current_page** | **int** |  | [optional] 
**data** | [**List[Model9946399cbddb0dcadcbd5801e5ee1dd4200ResponseDataInner]**](Model9946399cbddb0dcadcbd5801e5ee1dd4200ResponseDataInner.md) |  | [optional] 
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
from gateway_api_sdk.models.model9946399cbddb0dcadcbd5801e5ee1dd4200_response import Model9946399cbddb0dcadcbd5801e5ee1dd4200Response

# TODO update the JSON string below
json = "{}"
# create an instance of Model9946399cbddb0dcadcbd5801e5ee1dd4200Response from a JSON string
model9946399cbddb0dcadcbd5801e5ee1dd4200_response_instance = Model9946399cbddb0dcadcbd5801e5ee1dd4200Response.from_json(json)
# print the JSON string representation of the object
print(Model9946399cbddb0dcadcbd5801e5ee1dd4200Response.to_json())

# convert the object into a dict
model9946399cbddb0dcadcbd5801e5ee1dd4200_response_dict = model9946399cbddb0dcadcbd5801e5ee1dd4200_response_instance.to_dict()
# create an instance of Model9946399cbddb0dcadcbd5801e5ee1dd4200Response from a dict
model9946399cbddb0dcadcbd5801e5ee1dd4200_response_from_dict = Model9946399cbddb0dcadcbd5801e5ee1dd4200Response.from_dict(model9946399cbddb0dcadcbd5801e5ee1dd4200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


