# DataAccessApplicationReview

A review/comment thread against a single question of a Data Access Application

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**application_id** | **int** |  | [optional] 
**question_id** | **int** |  | [optional] 
**resolved** | **int** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**deleted_at** | **datetime** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.data_access_application_review import DataAccessApplicationReview

# TODO update the JSON string below
json = "{}"
# create an instance of DataAccessApplicationReview from a JSON string
data_access_application_review_instance = DataAccessApplicationReview.from_json(json)
# print the JSON string representation of the object
print(DataAccessApplicationReview.to_json())

# convert the object into a dict
data_access_application_review_dict = data_access_application_review_instance.to_dict()
# create an instance of DataAccessApplicationReview from a dict
data_access_application_review_from_dict = DataAccessApplicationReview.from_dict(data_access_application_review_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


