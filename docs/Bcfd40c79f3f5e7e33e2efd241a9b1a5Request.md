# Bcfd40c79f3f5e7e33e2efd241a9b1a5Request


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**applicant_id** | **int** |  | 
**submission_status** | **str** |  | 
**project_title** | **str** |  | [optional] 
**approval_status** | **str** |  | 
**team_ids** | **List[int]** |  | [optional] 
**answers** | [**List[Bcfd40c79f3f5e7e33e2efd241a9b1a5RequestAnswersInner]**](Bcfd40c79f3f5e7e33e2efd241a9b1a5RequestAnswersInner.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.bcfd40c79f3f5e7e33e2efd241a9b1a5_request import Bcfd40c79f3f5e7e33e2efd241a9b1a5Request

# TODO update the JSON string below
json = "{}"
# create an instance of Bcfd40c79f3f5e7e33e2efd241a9b1a5Request from a JSON string
bcfd40c79f3f5e7e33e2efd241a9b1a5_request_instance = Bcfd40c79f3f5e7e33e2efd241a9b1a5Request.from_json(json)
# print the JSON string representation of the object
print(Bcfd40c79f3f5e7e33e2efd241a9b1a5Request.to_json())

# convert the object into a dict
bcfd40c79f3f5e7e33e2efd241a9b1a5_request_dict = bcfd40c79f3f5e7e33e2efd241a9b1a5_request_instance.to_dict()
# create an instance of Bcfd40c79f3f5e7e33e2efd241a9b1a5Request from a dict
bcfd40c79f3f5e7e33e2efd241a9b1a5_request_from_dict = Bcfd40c79f3f5e7e33e2efd241a9b1a5Request.from_dict(bcfd40c79f3f5e7e33e2efd241a9b1a5_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


