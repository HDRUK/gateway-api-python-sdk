# RevokeAllTokensV2200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**RevokeAllTokensV2200ResponseData**](RevokeAllTokensV2200ResponseData.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.revoke_all_tokens_v2200_response import RevokeAllTokensV2200Response

# TODO update the JSON string below
json = "{}"
# create an instance of RevokeAllTokensV2200Response from a JSON string
revoke_all_tokens_v2200_response_instance = RevokeAllTokensV2200Response.from_json(json)
# print the JSON string representation of the object
print(RevokeAllTokensV2200Response.to_json())

# convert the object into a dict
revoke_all_tokens_v2200_response_dict = revoke_all_tokens_v2200_response_instance.to_dict()
# create an instance of RevokeAllTokensV2200Response from a dict
revoke_all_tokens_v2200_response_from_dict = RevokeAllTokensV2200Response.from_dict(revoke_all_tokens_v2200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


