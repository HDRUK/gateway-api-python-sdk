# CreateEnquiryThreadsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **int** |  | 
**project_title** | **str** |  | 
**is_dar_dialogue** | **bool** |  | [optional] 
**is_dar_status** | **bool** |  | [optional] 
**is_feasibility_enquiry** | **bool** |  | [optional] 
**is_general_enquiry** | **bool** |  | [optional] 
**is_dar_review** | **bool** |  | [optional] 
**enabled** | **bool** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_enquiry_threads_request import CreateEnquiryThreadsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateEnquiryThreadsRequest from a JSON string
create_enquiry_threads_request_instance = CreateEnquiryThreadsRequest.from_json(json)
# print the JSON string representation of the object
print(CreateEnquiryThreadsRequest.to_json())

# convert the object into a dict
create_enquiry_threads_request_dict = create_enquiry_threads_request_instance.to_dict()
# create an instance of CreateEnquiryThreadsRequest from a dict
create_enquiry_threads_request_from_dict = CreateEnquiryThreadsRequest.from_dict(create_enquiry_threads_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


