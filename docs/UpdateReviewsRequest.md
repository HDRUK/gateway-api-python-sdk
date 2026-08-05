# UpdateReviewsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tool_id** | **int** |  | [optional] 
**user_id** | **int** |  | [optional] 
**rating** | **int** |  | [optional] 
**review_text** | **str** |  | [optional] 
**review_state** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.update_reviews_request import UpdateReviewsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateReviewsRequest from a JSON string
update_reviews_request_instance = UpdateReviewsRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateReviewsRequest.to_json())

# convert the object into a dict
update_reviews_request_dict = update_reviews_request_instance.to_dict()
# create an instance of UpdateReviewsRequest from a dict
update_reviews_request_from_dict = UpdateReviewsRequest.from_dict(update_reviews_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


