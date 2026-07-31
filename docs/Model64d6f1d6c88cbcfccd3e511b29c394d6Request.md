# Model64d6f1d6c88cbcfccd3e511b29c394d6Request


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**section_id** | **int** |  | 
**user_id** | **int** |  | [optional] 
**team_ids** | **List[int]** |  | [optional] 
**locked** | **bool** |  | [optional] 
**archived** | **bool** |  | [optional] 
**is_child** | **bool** |  | [optional] 
**question_type** | **str** |  | [optional] 
**required** | **bool** |  | [optional] 
**force_required** | **bool** |  | 
**allow_guidance_override** | **bool** |  | 
**default** | **bool** |  | [optional] 
**guidance** | **str** |  | 
**title** | **str** |  | 
**var_field** | **List[object]** |  | 

## Example

```python
from gateway_api_sdk.models.model64d6f1d6c88cbcfccd3e511b29c394d6_request import Model64d6f1d6c88cbcfccd3e511b29c394d6Request

# TODO update the JSON string below
json = "{}"
# create an instance of Model64d6f1d6c88cbcfccd3e511b29c394d6Request from a JSON string
model64d6f1d6c88cbcfccd3e511b29c394d6_request_instance = Model64d6f1d6c88cbcfccd3e511b29c394d6Request.from_json(json)
# print the JSON string representation of the object
print(Model64d6f1d6c88cbcfccd3e511b29c394d6Request.to_json())

# convert the object into a dict
model64d6f1d6c88cbcfccd3e511b29c394d6_request_dict = model64d6f1d6c88cbcfccd3e511b29c394d6_request_instance.to_dict()
# create an instance of Model64d6f1d6c88cbcfccd3e511b29c394d6Request from a dict
model64d6f1d6c88cbcfccd3e511b29c394d6_request_from_dict = Model64d6f1d6c88cbcfccd3e511b29c394d6Request.from_dict(model64d6f1d6c88cbcfccd3e511b29c394d6_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


