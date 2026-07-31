# UpdateAdminSearchFeatureRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**feature** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.update_admin_search_feature_request import UpdateAdminSearchFeatureRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateAdminSearchFeatureRequest from a JSON string
update_admin_search_feature_request_instance = UpdateAdminSearchFeatureRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateAdminSearchFeatureRequest.to_json())

# convert the object into a dict
update_admin_search_feature_request_dict = update_admin_search_feature_request_instance.to_dict()
# create an instance of UpdateAdminSearchFeatureRequest from a dict
update_admin_search_feature_request_from_dict = UpdateAdminSearchFeatureRequest.from_dict(update_admin_search_feature_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


