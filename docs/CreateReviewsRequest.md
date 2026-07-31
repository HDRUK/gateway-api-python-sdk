# CreateReviewsRequest


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
from gateway_api_sdk.models.create_reviews_request import CreateReviewsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateReviewsRequest from a JSON string
create_reviews_request_instance = CreateReviewsRequest.from_json(json)
# print the JSON string representation of the object
print(CreateReviewsRequest.to_json())

# convert the object into a dict
create_reviews_request_dict = create_reviews_request_instance.to_dict()
# create an instance of CreateReviewsRequest from a dict
create_reviews_request_from_dict = CreateReviewsRequest.from_dict(create_reviews_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


