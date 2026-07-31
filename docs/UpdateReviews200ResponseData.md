# UpdateReviews200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**tool_id** | **int** |  | [optional] 
**user_id** | **int** |  | [optional] 
**rating** | **int** |  | [optional] 
**review_text** | **str** |  | [optional] 
**review_state** | **str** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**deleted_at** | **datetime** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.update_reviews200_response_data import UpdateReviews200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateReviews200ResponseData from a JSON string
update_reviews200_response_data_instance = UpdateReviews200ResponseData.from_json(json)
# print the JSON string representation of the object
print(UpdateReviews200ResponseData.to_json())

# convert the object into a dict
update_reviews200_response_data_dict = update_reviews200_response_data_instance.to_dict()
# create an instance of UpdateReviews200ResponseData from a dict
update_reviews200_response_data_from_dict = UpdateReviews200ResponseData.from_dict(update_reviews200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


