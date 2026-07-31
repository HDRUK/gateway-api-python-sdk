# FetchFiles200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**filename** | **str** |  | [optional] 
**file_location** | **str** |  | [optional] 
**user_id** | **str** |  | [optional] 
**status** | **str** |  | [optional] 
**error** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_files200_response_data_inner import FetchFiles200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of FetchFiles200ResponseDataInner from a JSON string
fetch_files200_response_data_inner_instance = FetchFiles200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(FetchFiles200ResponseDataInner.to_json())

# convert the object into a dict
fetch_files200_response_data_inner_dict = fetch_files200_response_data_inner_instance.to_dict()
# create an instance of FetchFiles200ResponseDataInner from a dict
fetch_files200_response_data_inner_from_dict = FetchFiles200ResponseDataInner.from_dict(fetch_files200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


