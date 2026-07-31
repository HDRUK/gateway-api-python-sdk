# CreateDurRequestPublicationsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**reason** | **str** |  | [optional] 
**user_id** | **int** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_dur_request_publications_inner import CreateDurRequestPublicationsInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateDurRequestPublicationsInner from a JSON string
create_dur_request_publications_inner_instance = CreateDurRequestPublicationsInner.from_json(json)
# print the JSON string representation of the object
print(CreateDurRequestPublicationsInner.to_json())

# convert the object into a dict
create_dur_request_publications_inner_dict = create_dur_request_publications_inner_instance.to_dict()
# create an instance of CreateDurRequestPublicationsInner from a dict
create_dur_request_publications_inner_from_dict = CreateDurRequestPublicationsInner.from_dict(create_dur_request_publications_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


