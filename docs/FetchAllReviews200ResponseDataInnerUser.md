# FetchAllReviews200ResponseDataInnerUser


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**name** | **str** |  | [optional] 
**firstname** | **str** |  | [optional] 
**lastname** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**email_verified_at** | **int** |  | [optional] 
**providerid** | **str** |  | [optional] 
**provider** | **str** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**deleted_at** | **datetime** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_all_reviews200_response_data_inner_user import FetchAllReviews200ResponseDataInnerUser

# TODO update the JSON string below
json = "{}"
# create an instance of FetchAllReviews200ResponseDataInnerUser from a JSON string
fetch_all_reviews200_response_data_inner_user_instance = FetchAllReviews200ResponseDataInnerUser.from_json(json)
# print the JSON string representation of the object
print(FetchAllReviews200ResponseDataInnerUser.to_json())

# convert the object into a dict
fetch_all_reviews200_response_data_inner_user_dict = fetch_all_reviews200_response_data_inner_user_instance.to_dict()
# create an instance of FetchAllReviews200ResponseDataInnerUser from a dict
fetch_all_reviews200_response_data_inner_user_from_dict = FetchAllReviews200ResponseDataInnerUser.from_dict(fetch_all_reviews200_response_data_inner_user_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


