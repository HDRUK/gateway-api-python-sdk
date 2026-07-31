# FetchAllReviews200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**tool_id** | **int** |  | [optional] 
**user_id** | **int** |  | [optional] 
**rating** | **int** |  | [optional] 
**review_text** | **str** |  | [optional] 
**review_state** | **int** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**deleted_at** | **datetime** |  | [optional] 
**tool** | [**FetchAllReviews200ResponseDataInnerTool**](FetchAllReviews200ResponseDataInnerTool.md) |  | [optional] 
**user** | [**FetchAllReviews200ResponseDataInnerUser**](FetchAllReviews200ResponseDataInnerUser.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_all_reviews200_response_data_inner import FetchAllReviews200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of FetchAllReviews200ResponseDataInner from a JSON string
fetch_all_reviews200_response_data_inner_instance = FetchAllReviews200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(FetchAllReviews200ResponseDataInner.to_json())

# convert the object into a dict
fetch_all_reviews200_response_data_inner_dict = fetch_all_reviews200_response_data_inner_instance.to_dict()
# create an instance of FetchAllReviews200ResponseDataInner from a dict
fetch_all_reviews200_response_data_inner_from_dict = FetchAllReviews200ResponseDataInner.from_dict(fetch_all_reviews200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


