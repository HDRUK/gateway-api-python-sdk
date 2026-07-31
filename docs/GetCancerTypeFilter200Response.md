# GetCancerTypeFilter200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GetCancerTypeFilters200ResponseDataInner**](GetCancerTypeFilters200ResponseDataInner.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.get_cancer_type_filter200_response import GetCancerTypeFilter200Response

# TODO update the JSON string below
json = "{}"
# create an instance of GetCancerTypeFilter200Response from a JSON string
get_cancer_type_filter200_response_instance = GetCancerTypeFilter200Response.from_json(json)
# print the JSON string representation of the object
print(GetCancerTypeFilter200Response.to_json())

# convert the object into a dict
get_cancer_type_filter200_response_dict = get_cancer_type_filter200_response_instance.to_dict()
# create an instance of GetCancerTypeFilter200Response from a dict
get_cancer_type_filter200_response_from_dict = GetCancerTypeFilter200Response.from_dict(get_cancer_type_filter200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


