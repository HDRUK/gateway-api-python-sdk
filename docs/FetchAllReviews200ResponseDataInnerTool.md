# FetchAllReviews200ResponseDataInnerTool


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**mongo_object_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**url** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**license** | **str** |  | [optional] 
**tech_stack** | **str** |  | [optional] 
**user_id** | **int** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**deleted_at** | **datetime** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_all_reviews200_response_data_inner_tool import FetchAllReviews200ResponseDataInnerTool

# TODO update the JSON string below
json = "{}"
# create an instance of FetchAllReviews200ResponseDataInnerTool from a JSON string
fetch_all_reviews200_response_data_inner_tool_instance = FetchAllReviews200ResponseDataInnerTool.from_json(json)
# print the JSON string representation of the object
print(FetchAllReviews200ResponseDataInnerTool.to_json())

# convert the object into a dict
fetch_all_reviews200_response_data_inner_tool_dict = fetch_all_reviews200_response_data_inner_tool_instance.to_dict()
# create an instance of FetchAllReviews200ResponseDataInnerTool from a dict
fetch_all_reviews200_response_data_inner_tool_from_dict = FetchAllReviews200ResponseDataInnerTool.from_dict(fetch_all_reviews200_response_data_inner_tool_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


