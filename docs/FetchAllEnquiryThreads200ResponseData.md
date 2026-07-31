# FetchAllEnquiryThreads200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**user_id** | **int** |  | [optional] 
**team_id** | **int** |  | [optional] 
**project_title** | **str** |  | [optional] 
**unique_id** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_all_enquiry_threads200_response_data import FetchAllEnquiryThreads200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of FetchAllEnquiryThreads200ResponseData from a JSON string
fetch_all_enquiry_threads200_response_data_instance = FetchAllEnquiryThreads200ResponseData.from_json(json)
# print the JSON string representation of the object
print(FetchAllEnquiryThreads200ResponseData.to_json())

# convert the object into a dict
fetch_all_enquiry_threads200_response_data_dict = fetch_all_enquiry_threads200_response_data_instance.to_dict()
# create an instance of FetchAllEnquiryThreads200ResponseData from a dict
fetch_all_enquiry_threads200_response_data_from_dict = FetchAllEnquiryThreads200ResponseData.from_dict(fetch_all_enquiry_threads200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


