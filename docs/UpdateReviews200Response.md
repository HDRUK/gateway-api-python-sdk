# UpdateReviews200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**UpdateReviews200ResponseData**](UpdateReviews200ResponseData.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.update_reviews200_response import UpdateReviews200Response

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateReviews200Response from a JSON string
update_reviews200_response_instance = UpdateReviews200Response.from_json(json)
# print the JSON string representation of the object
print(UpdateReviews200Response.to_json())

# convert the object into a dict
update_reviews200_response_dict = update_reviews200_response_instance.to_dict()
# create an instance of UpdateReviews200Response from a dict
update_reviews200_response_from_dict = UpdateReviews200Response.from_dict(update_reviews200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


