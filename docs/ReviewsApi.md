# gateway_api_sdk.ReviewsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**call_205dc23d44b18ca0b5c26a293cc69cf7**](ReviewsApi.md#call_205dc23d44b18ca0b5c26a293cc69cf7) | **DELETE** /api/v1/reviews/{id} | Delete a review
[**call_31ad2467e98e52298b4e39e2741447f1**](ReviewsApi.md#call_31ad2467e98e52298b4e39e2741447f1) | **PATCH** /api/v1/reviews/{id} | Edit a review
[**call_64b4b952592ebe8e0b00204e76bd991c**](ReviewsApi.md#call_64b4b952592ebe8e0b00204e76bd991c) | **PUT** /api/v1/reviews/{id} | Update a review
[**create_reviews**](ReviewsApi.md#create_reviews) | **POST** /api/v1/reviews | ReviewController@store
[**fetch_all_reviews**](ReviewsApi.md#fetch_all_reviews) | **GET** /api/v1/reviews | ReviewController@index
[**fetch_reviews**](ReviewsApi.md#fetch_reviews) | **GET** /api/v1/reviews/{id} | ReviewController@show


# **call_205dc23d44b18ca0b5c26a293cc69cf7**
> C29b5b3424f7317b69b4bda048ccfafb200Response call_205dc23d44b18ca0b5c26a293cc69cf7(id)

Delete a review

Delete a review

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.c29b5b3424f7317b69b4bda048ccfafb200_response import C29b5b3424f7317b69b4bda048ccfafb200Response
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
        api_response = api_instance.call_205dc23d44b18ca0b5c26a293cc69cf7(id)
        print("The response of ReviewsApi->call_205dc23d44b18ca0b5c26a293cc69cf7:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReviewsApi->call_205dc23d44b18ca0b5c26a293cc69cf7: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| review id | 

### Return type

[**C29b5b3424f7317b69b4bda048ccfafb200Response**](C29b5b3424f7317b69b4bda048ccfafb200Response.md)

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

# **call_31ad2467e98e52298b4e39e2741447f1**
> Model64b4b952592ebe8e0b00204e76bd991c200Response call_31ad2467e98e52298b4e39e2741447f1(id, create_reviews_request)

Edit a review

Edit a review

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_reviews_request import CreateReviewsRequest
from gateway_api_sdk.models.model64b4b952592ebe8e0b00204e76bd991c200_response import Model64b4b952592ebe8e0b00204e76bd991c200Response
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
    create_reviews_request = gateway_api_sdk.CreateReviewsRequest() # CreateReviewsRequest | Pass user credentials

    try:
        # Edit a review
        api_response = api_instance.call_31ad2467e98e52298b4e39e2741447f1(id, create_reviews_request)
        print("The response of ReviewsApi->call_31ad2467e98e52298b4e39e2741447f1:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReviewsApi->call_31ad2467e98e52298b4e39e2741447f1: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| review id | 
 **create_reviews_request** | [**CreateReviewsRequest**](CreateReviewsRequest.md)| Pass user credentials | 

### Return type

[**Model64b4b952592ebe8e0b00204e76bd991c200Response**](Model64b4b952592ebe8e0b00204e76bd991c200Response.md)

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

# **call_64b4b952592ebe8e0b00204e76bd991c**
> Model64b4b952592ebe8e0b00204e76bd991c200Response call_64b4b952592ebe8e0b00204e76bd991c(id, create_reviews_request)

Update a review

Update a review

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_reviews_request import CreateReviewsRequest
from gateway_api_sdk.models.model64b4b952592ebe8e0b00204e76bd991c200_response import Model64b4b952592ebe8e0b00204e76bd991c200Response
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
    create_reviews_request = gateway_api_sdk.CreateReviewsRequest() # CreateReviewsRequest | Pass user credentials

    try:
        # Update a review
        api_response = api_instance.call_64b4b952592ebe8e0b00204e76bd991c(id, create_reviews_request)
        print("The response of ReviewsApi->call_64b4b952592ebe8e0b00204e76bd991c:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReviewsApi->call_64b4b952592ebe8e0b00204e76bd991c: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| review id | 
 **create_reviews_request** | [**CreateReviewsRequest**](CreateReviewsRequest.md)| Pass user credentials | 

### Return type

[**Model64b4b952592ebe8e0b00204e76bd991c200Response**](Model64b4b952592ebe8e0b00204e76bd991c200Response.md)

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

# **create_reviews**
> Dd76b8d73b7ea8b4951f03d7c0904c92200Response create_reviews(create_reviews_request)

ReviewController@store

Create a new review

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_reviews_request import CreateReviewsRequest
from gateway_api_sdk.models.dd76b8d73b7ea8b4951f03d7c0904c92200_response import Dd76b8d73b7ea8b4951f03d7c0904c92200Response
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
    create_reviews_request = gateway_api_sdk.CreateReviewsRequest() # CreateReviewsRequest | Pass user credentials

    try:
        # ReviewController@store
        api_response = api_instance.create_reviews(create_reviews_request)
        print("The response of ReviewsApi->create_reviews:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReviewsApi->create_reviews: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_reviews_request** | [**CreateReviewsRequest**](CreateReviewsRequest.md)| Pass user credentials | 

### Return type

[**Dd76b8d73b7ea8b4951f03d7c0904c92200Response**](Dd76b8d73b7ea8b4951f03d7c0904c92200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Created |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_all_reviews**
> FetchAllReviews200Response fetch_all_reviews()

ReviewController@index

Get All Reviews

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_reviews200_response import FetchAllReviews200Response
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

    try:
        # ReviewController@index
        api_response = api_instance.fetch_all_reviews()
        print("The response of ReviewsApi->fetch_all_reviews:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReviewsApi->fetch_all_reviews: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**FetchAllReviews200Response**](FetchAllReviews200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_reviews**
> FetchAllReviews200Response fetch_reviews(id)

ReviewController@show

Get review by id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_reviews200_response import FetchAllReviews200Response
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
        # ReviewController@show
        api_response = api_instance.fetch_reviews(id)
        print("The response of ReviewsApi->fetch_reviews:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReviewsApi->fetch_reviews: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| review id | 

### Return type

[**FetchAllReviews200Response**](FetchAllReviews200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |
**401** | Unauthorized |  -  |
**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

