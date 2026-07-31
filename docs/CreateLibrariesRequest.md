# CreateLibrariesRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**dataset_id** | **int** |  | 

## Example

```python
from gateway_api_sdk.models.create_libraries_request import CreateLibrariesRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateLibrariesRequest from a JSON string
create_libraries_request_instance = CreateLibrariesRequest.from_json(json)
# print the JSON string representation of the object
print(CreateLibrariesRequest.to_json())

# convert the object into a dict
create_libraries_request_dict = create_libraries_request_instance.to_dict()
# create an instance of CreateLibrariesRequest from a dict
create_libraries_request_from_dict = CreateLibrariesRequest.from_dict(create_libraries_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


