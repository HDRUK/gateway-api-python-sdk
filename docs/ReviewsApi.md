# gateway_api_sdk.ReviewsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_reviews**](ReviewsApi.md#delete_reviews) | **DELETE** /api/v1/reviews/{id} | Delete a review
[**edit_reviews**](ReviewsApi.md#edit_reviews) | **PATCH** /api/v1/reviews/{id} | Edit a review
[**update_reviews**](ReviewsApi.md#update_reviews) | **PUT** /api/v1/reviews/{id} | Update a review


# **delete_reviews**
> DeleteApplications200Response delete_reviews(id)

Delete a review

Delete a review

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.delete_applications200_response import DeleteApplications200Response
from gateway_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = gateway_api_sdk.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): bearerAuth
configuration = gateway_api_sdk.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with gateway_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = gateway_api_sdk.ReviewsApi(api_client)
    id = 1 # int | review id

    try:
        # Delete a review
        api_response = api_instance.delete_reviews(id)
        print("The response of ReviewsApi->delete_reviews:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReviewsApi->delete_reviews: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| review id | 

### Return type

[**DeleteApplications200Response**](DeleteApplications200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**404** | Not found response |  -  |
**200** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **edit_reviews**
> UpdateReviews200Response edit_reviews(id, update_reviews_request)

Edit a review

Edit a review

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.update_reviews200_response import UpdateReviews200Response
from gateway_api_sdk.models.update_reviews_request import UpdateReviewsRequest
from gateway_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = gateway_api_sdk.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): bearerAuth
configuration = gateway_api_sdk.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with gateway_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = gateway_api_sdk.ReviewsApi(api_client)
    id = 1 # int | review id
    update_reviews_request = gateway_api_sdk.UpdateReviewsRequest() # UpdateReviewsRequest | Pass user credentials

    try:
        # Edit a review
        api_response = api_instance.edit_reviews(id, update_reviews_request)
        print("The response of ReviewsApi->edit_reviews:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReviewsApi->edit_reviews: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| review id | 
 **update_reviews_request** | [**UpdateReviewsRequest**](UpdateReviewsRequest.md)| Pass user credentials | 

### Return type

[**UpdateReviews200Response**](UpdateReviews200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**404** | Not found response |  -  |
**200** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_reviews**
> UpdateReviews200Response update_reviews(id, update_reviews_request)

Update a review

Update a review

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.update_reviews200_response import UpdateReviews200Response
from gateway_api_sdk.models.update_reviews_request import UpdateReviewsRequest
from gateway_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = gateway_api_sdk.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): bearerAuth
configuration = gateway_api_sdk.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with gateway_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = gateway_api_sdk.ReviewsApi(api_client)
    id = 1 # int | review id
    update_reviews_request = gateway_api_sdk.UpdateReviewsRequest() # UpdateReviewsRequest | Pass user credentials

    try:
        # Update a review
        api_response = api_instance.update_reviews(id, update_reviews_request)
        print("The response of ReviewsApi->update_reviews:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReviewsApi->update_reviews: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| review id | 
 **update_reviews_request** | [**UpdateReviewsRequest**](UpdateReviewsRequest.md)| Pass user credentials | 

### Return type

[**UpdateReviews200Response**](UpdateReviews200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**404** | Not found response |  -  |
**200** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

