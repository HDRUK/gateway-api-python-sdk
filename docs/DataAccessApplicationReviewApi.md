# gateway_api_sdk.DataAccessApplicationReviewApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_team_dar_application_question_review**](DataAccessApplicationReviewApi.md#create_team_dar_application_question_review) | **POST** /api/v1/teams/{team_id}/dar/applications/{id}/questions/{questionId}/reviews | DataAccessApplicationReview@store
[**create_team_dar_application_review**](DataAccessApplicationReviewApi.md#create_team_dar_application_review) | **POST** /api/v1/teams/{team_id}/dar/applications/{id}/reviews | DataAccessApplicationReview@storeGlobal
[**delete_team_dar_application_question_review**](DataAccessApplicationReviewApi.md#delete_team_dar_application_question_review) | **DELETE** /api/v1/teams/{team_id}/dar/applications/{id}/questions/{questionId}/reviews/{reviewId} | DataAccessApplicationReview@destroy
[**delete_team_dar_application_review**](DataAccessApplicationReviewApi.md#delete_team_dar_application_review) | **DELETE** /api/v1/teams/{team_id}/dar/applications/{id}/reviews/{reviewId} | DataAccessApplicationReview@destroyGlobal
[**delete_team_dar_application_review_file**](DataAccessApplicationReviewApi.md#delete_team_dar_application_review_file) | **DELETE** /api/v1/teams/{teamId}/dar/applications/{id}/reviews/{reviewId}/files/{fileId} | DataAccessApplicationReview@destroyFile
[**fetch_team_dar_application_review_file**](DataAccessApplicationReviewApi.md#fetch_team_dar_application_review_file) | **GET** /ap1/v1/teams/{teamId}/dar/applications/{id}/reviews/{reviewId}/download/{fileId} | DataAccessApplicationReview@downloadFile
[**fetch_team_dar_application_reviews**](DataAccessApplicationReviewApi.md#fetch_team_dar_application_reviews) | **GET** /api/v1/teams/{team_id}/dar/applications/{id}/reviews | DataAccessApplicationReview@index
[**fetch_user_dar_application_review_file**](DataAccessApplicationReviewApi.md#fetch_user_dar_application_review_file) | **GET** /ap1/v1/users/{userId}/dar/applications/{id}/reviews/{reviewId}/download/{fileId} | DataAccessApplicationReview@downloadUserFile
[**fetch_user_dar_application_reviews**](DataAccessApplicationReviewApi.md#fetch_user_dar_application_reviews) | **GET** /api/v1/users/{userId}/dar/applications/{id}/reviews | DataAccessApplicationReview@index
[**update_team_dar_application_question_review**](DataAccessApplicationReviewApi.md#update_team_dar_application_question_review) | **PUT** /api/v1/teams/{team_id}/dar/applications/{id}/questions/{questionId}/reviews/{reviewId} | DataAccessApplicationReview@update
[**update_team_dar_application_review**](DataAccessApplicationReviewApi.md#update_team_dar_application_review) | **PUT** /api/v1/teams/{team_id}/dar/applications/{id}/reviews/{reviewId} | DataAccessApplicationReview@updateGlobal
[**update_user_dar_application_question_review**](DataAccessApplicationReviewApi.md#update_user_dar_application_question_review) | **PUT** /api/v1/users/{userId}/dar/applications/{id}/questions/{questionId}/reviews/{reviewId} | DataAccessApplicationReview@userUpdate
[**update_user_dar_application_review**](DataAccessApplicationReviewApi.md#update_user_dar_application_review) | **PUT** /api/v1/users/{userId}/dar/applications/{id}/reviews/{reviewId} | DataAccessApplicationReview@userUpdateGlobal


# **create_team_dar_application_question_review**
> CreateCategories200Response create_team_dar_application_question_review(team_id, id, question_id, create_team_dar_application_review_request)

DataAccessApplicationReview@store

Create a new review comment on a question in a DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_categories200_response import CreateCategories200Response
from gateway_api_sdk.models.create_team_dar_application_review_request import CreateTeamDarApplicationReviewRequest
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
    api_instance = gateway_api_sdk.DataAccessApplicationReviewApi(api_client)
    team_id = 1 # int | Team id
    id = 1 # int | DAR application id
    question_id = 1 # int | DAR application question id
    create_team_dar_application_review_request = gateway_api_sdk.CreateTeamDarApplicationReviewRequest() # CreateTeamDarApplicationReviewRequest | DataAccessApplicationReview definition

    try:
        # DataAccessApplicationReview@store
        api_response = api_instance.create_team_dar_application_question_review(team_id, id, question_id, create_team_dar_application_review_request)
        print("The response of DataAccessApplicationReviewApi->create_team_dar_application_question_review:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationReviewApi->create_team_dar_application_question_review: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **id** | **int**| DAR application id | 
 **question_id** | **int**| DAR application question id | 
 **create_team_dar_application_review_request** | [**CreateTeamDarApplicationReviewRequest**](CreateTeamDarApplicationReviewRequest.md)| DataAccessApplicationReview definition | 

### Return type

[**CreateCategories200Response**](CreateCategories200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_team_dar_application_review**
> CreateCategories200Response create_team_dar_application_review(team_id, id, create_team_dar_application_review_request)

DataAccessApplicationReview@storeGlobal

Create a new review comment on a DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_categories200_response import CreateCategories200Response
from gateway_api_sdk.models.create_team_dar_application_review_request import CreateTeamDarApplicationReviewRequest
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
    api_instance = gateway_api_sdk.DataAccessApplicationReviewApi(api_client)
    team_id = 1 # int | Team id
    id = 1 # int | DAR application id
    create_team_dar_application_review_request = gateway_api_sdk.CreateTeamDarApplicationReviewRequest() # CreateTeamDarApplicationReviewRequest | DataAccessApplicationReview definition

    try:
        # DataAccessApplicationReview@storeGlobal
        api_response = api_instance.create_team_dar_application_review(team_id, id, create_team_dar_application_review_request)
        print("The response of DataAccessApplicationReviewApi->create_team_dar_application_review:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationReviewApi->create_team_dar_application_review: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **id** | **int**| DAR application id | 
 **create_team_dar_application_review_request** | [**CreateTeamDarApplicationReviewRequest**](CreateTeamDarApplicationReviewRequest.md)| DataAccessApplicationReview definition | 

### Return type

[**CreateCategories200Response**](CreateCategories200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_team_dar_application_question_review**
> DeleteAliases200Response delete_team_dar_application_question_review(team_id, id, question_id, review_id)

DataAccessApplicationReview@destroy

Delete a review from a DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.delete_aliases200_response import DeleteAliases200Response
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
    api_instance = gateway_api_sdk.DataAccessApplicationReviewApi(api_client)
    team_id = 1 # int | Team id
    id = 1 # int | DAR application id
    question_id = 1 # int | DAR application question id
    review_id = 1 # int | DAR application review id

    try:
        # DataAccessApplicationReview@destroy
        api_response = api_instance.delete_team_dar_application_question_review(team_id, id, question_id, review_id)
        print("The response of DataAccessApplicationReviewApi->delete_team_dar_application_question_review:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationReviewApi->delete_team_dar_application_question_review: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **id** | **int**| DAR application id | 
 **question_id** | **int**| DAR application question id | 
 **review_id** | **int**| DAR application review id | 

### Return type

[**DeleteAliases200Response**](DeleteAliases200Response.md)

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

# **delete_team_dar_application_review**
> DeleteAliases200Response delete_team_dar_application_review(team_id, id, review_id)

DataAccessApplicationReview@destroyGlobal

Delete a review from a DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.delete_aliases200_response import DeleteAliases200Response
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
    api_instance = gateway_api_sdk.DataAccessApplicationReviewApi(api_client)
    team_id = 1 # int | Team id
    id = 1 # int | DAR application id
    review_id = 1 # int | DAR application review id

    try:
        # DataAccessApplicationReview@destroyGlobal
        api_response = api_instance.delete_team_dar_application_review(team_id, id, review_id)
        print("The response of DataAccessApplicationReviewApi->delete_team_dar_application_review:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationReviewApi->delete_team_dar_application_review: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **id** | **int**| DAR application id | 
 **review_id** | **int**| DAR application review id | 

### Return type

[**DeleteAliases200Response**](DeleteAliases200Response.md)

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

# **delete_team_dar_application_review_file**
> DeleteAliases200Response delete_team_dar_application_review_file(team_id, id, review_id, file_id)

DataAccessApplicationReview@destroyFile

Delete a file associated with a DAR review

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.delete_aliases200_response import DeleteAliases200Response
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
    api_instance = gateway_api_sdk.DataAccessApplicationReviewApi(api_client)
    team_id = 1 # int | Team id
    id = 1 # int | Dar application id
    review_id = 1 # int | Review id
    file_id = '1' # str | File uuid

    try:
        # DataAccessApplicationReview@destroyFile
        api_response = api_instance.delete_team_dar_application_review_file(team_id, id, review_id, file_id)
        print("The response of DataAccessApplicationReviewApi->delete_team_dar_application_review_file:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationReviewApi->delete_team_dar_application_review_file: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **id** | **int**| Dar application id | 
 **review_id** | **int**| Review id | 
 **file_id** | **str**| File uuid | 

### Return type

[**DeleteAliases200Response**](DeleteAliases200Response.md)

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

# **fetch_team_dar_application_review_file**
> fetch_team_dar_application_review_file(team_id, id, review_id, file_id)

DataAccessApplicationReview@downloadFile

Download a file associated with a DAR application review

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
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
    api_instance = gateway_api_sdk.DataAccessApplicationReviewApi(api_client)
    team_id = 1 # int | Team id
    id = 1 # int | DAR application id
    review_id = 1 # int | DAR application review id
    file_id = '1' # str | File uuid

    try:
        # DataAccessApplicationReview@downloadFile
        api_instance.fetch_team_dar_application_review_file(team_id, id, review_id, file_id)
    except Exception as e:
        print("Exception when calling DataAccessApplicationReviewApi->fetch_team_dar_application_review_file: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **id** | **int**| DAR application id | 
 **review_id** | **int**| DAR application review id | 
 **file_id** | **str**| File uuid | 

### Return type

void (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: file, application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_team_dar_application_reviews**
> FetchTeamDarApplicationReviews200Response fetch_team_dar_application_reviews(team_id, id)

DataAccessApplicationReview@index

Return all reviews on a DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_team_dar_application_reviews200_response import FetchTeamDarApplicationReviews200Response
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
    api_instance = gateway_api_sdk.DataAccessApplicationReviewApi(api_client)
    team_id = 1 # int | Team id
    id = 1 # int | DAR application id

    try:
        # DataAccessApplicationReview@index
        api_response = api_instance.fetch_team_dar_application_reviews(team_id, id)
        print("The response of DataAccessApplicationReviewApi->fetch_team_dar_application_reviews:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationReviewApi->fetch_team_dar_application_reviews: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **id** | **int**| DAR application id | 

### Return type

[**FetchTeamDarApplicationReviews200Response**](FetchTeamDarApplicationReviews200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_user_dar_application_review_file**
> fetch_user_dar_application_review_file(user_id, id, review_id, file_id)

DataAccessApplicationReview@downloadUserFile

Download a file associated with a DAR application review

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
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
    api_instance = gateway_api_sdk.DataAccessApplicationReviewApi(api_client)
    user_id = 1 # int | User id
    id = 1 # int | DAR application id
    review_id = 1 # int | DAR application review id
    file_id = '1' # str | File uuid

    try:
        # DataAccessApplicationReview@downloadUserFile
        api_instance.fetch_user_dar_application_review_file(user_id, id, review_id, file_id)
    except Exception as e:
        print("Exception when calling DataAccessApplicationReviewApi->fetch_user_dar_application_review_file: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| User id | 
 **id** | **int**| DAR application id | 
 **review_id** | **int**| DAR application review id | 
 **file_id** | **str**| File uuid | 

### Return type

void (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: file, application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_user_dar_application_reviews**
> FetchTeamDarApplicationReviews200Response fetch_user_dar_application_reviews(user_id, id)

DataAccessApplicationReview@index

Return all reviews on a DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_team_dar_application_reviews200_response import FetchTeamDarApplicationReviews200Response
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
    api_instance = gateway_api_sdk.DataAccessApplicationReviewApi(api_client)
    user_id = 1 # int | User id
    id = 1 # int | DAR application id

    try:
        # DataAccessApplicationReview@index
        api_response = api_instance.fetch_user_dar_application_reviews(user_id, id)
        print("The response of DataAccessApplicationReviewApi->fetch_user_dar_application_reviews:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationReviewApi->fetch_user_dar_application_reviews: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| User id | 
 **id** | **int**| DAR application id | 

### Return type

[**FetchTeamDarApplicationReviews200Response**](FetchTeamDarApplicationReviews200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_team_dar_application_question_review**
> UpdateTeamDarApplicationQuestionReview200Response update_team_dar_application_question_review(team_id, id, question_id, review_id, create_team_dar_application_review_request)

DataAccessApplicationReview@update

Update a review comment on a question in a DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_team_dar_application_review_request import CreateTeamDarApplicationReviewRequest
from gateway_api_sdk.models.update_team_dar_application_question_review200_response import UpdateTeamDarApplicationQuestionReview200Response
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
    api_instance = gateway_api_sdk.DataAccessApplicationReviewApi(api_client)
    team_id = 1 # int | Team id
    id = 1 # int | DAR application id
    question_id = 1 # int | DAR application question id
    review_id = 1 # int | DAR application review id
    create_team_dar_application_review_request = gateway_api_sdk.CreateTeamDarApplicationReviewRequest() # CreateTeamDarApplicationReviewRequest | DataAccessApplicationReview definition

    try:
        # DataAccessApplicationReview@update
        api_response = api_instance.update_team_dar_application_question_review(team_id, id, question_id, review_id, create_team_dar_application_review_request)
        print("The response of DataAccessApplicationReviewApi->update_team_dar_application_question_review:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationReviewApi->update_team_dar_application_question_review: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **id** | **int**| DAR application id | 
 **question_id** | **int**| DAR application question id | 
 **review_id** | **int**| DAR application review id | 
 **create_team_dar_application_review_request** | [**CreateTeamDarApplicationReviewRequest**](CreateTeamDarApplicationReviewRequest.md)| DataAccessApplicationReview definition | 

### Return type

[**UpdateTeamDarApplicationQuestionReview200Response**](UpdateTeamDarApplicationQuestionReview200Response.md)

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

# **update_team_dar_application_review**
> UpdateTeamDarApplicationQuestionReview200Response update_team_dar_application_review(team_id, id, review_id, create_team_dar_application_review_request)

DataAccessApplicationReview@updateGlobal

Update a review comment on a DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_team_dar_application_review_request import CreateTeamDarApplicationReviewRequest
from gateway_api_sdk.models.update_team_dar_application_question_review200_response import UpdateTeamDarApplicationQuestionReview200Response
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
    api_instance = gateway_api_sdk.DataAccessApplicationReviewApi(api_client)
    team_id = 1 # int | Team id
    id = 1 # int | DAR application id
    review_id = 1 # int | DAR application review id
    create_team_dar_application_review_request = gateway_api_sdk.CreateTeamDarApplicationReviewRequest() # CreateTeamDarApplicationReviewRequest | DataAccessApplicationReview definition

    try:
        # DataAccessApplicationReview@updateGlobal
        api_response = api_instance.update_team_dar_application_review(team_id, id, review_id, create_team_dar_application_review_request)
        print("The response of DataAccessApplicationReviewApi->update_team_dar_application_review:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationReviewApi->update_team_dar_application_review: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **id** | **int**| DAR application id | 
 **review_id** | **int**| DAR application review id | 
 **create_team_dar_application_review_request** | [**CreateTeamDarApplicationReviewRequest**](CreateTeamDarApplicationReviewRequest.md)| DataAccessApplicationReview definition | 

### Return type

[**UpdateTeamDarApplicationQuestionReview200Response**](UpdateTeamDarApplicationQuestionReview200Response.md)

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

# **update_user_dar_application_question_review**
> UpdateTeamDarApplicationQuestionReview200Response update_user_dar_application_question_review(user_id, id, question_id, review_id, create_team_dar_application_review_request)

DataAccessApplicationReview@userUpdate

User endpoint to update a review comment on a question in a DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_team_dar_application_review_request import CreateTeamDarApplicationReviewRequest
from gateway_api_sdk.models.update_team_dar_application_question_review200_response import UpdateTeamDarApplicationQuestionReview200Response
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
    api_instance = gateway_api_sdk.DataAccessApplicationReviewApi(api_client)
    user_id = 1 # int | User id
    id = 1 # int | DAR application id
    question_id = 1 # int | DAR application question id
    review_id = 1 # int | DAR application review id
    create_team_dar_application_review_request = gateway_api_sdk.CreateTeamDarApplicationReviewRequest() # CreateTeamDarApplicationReviewRequest | DataAccessApplicationReview definition

    try:
        # DataAccessApplicationReview@userUpdate
        api_response = api_instance.update_user_dar_application_question_review(user_id, id, question_id, review_id, create_team_dar_application_review_request)
        print("The response of DataAccessApplicationReviewApi->update_user_dar_application_question_review:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationReviewApi->update_user_dar_application_question_review: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| User id | 
 **id** | **int**| DAR application id | 
 **question_id** | **int**| DAR application question id | 
 **review_id** | **int**| DAR application review id | 
 **create_team_dar_application_review_request** | [**CreateTeamDarApplicationReviewRequest**](CreateTeamDarApplicationReviewRequest.md)| DataAccessApplicationReview definition | 

### Return type

[**UpdateTeamDarApplicationQuestionReview200Response**](UpdateTeamDarApplicationQuestionReview200Response.md)

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

# **update_user_dar_application_review**
> UpdateTeamDarApplicationQuestionReview200Response update_user_dar_application_review(user_id, id, review_id, create_team_dar_application_review_request)

DataAccessApplicationReview@userUpdateGlobal

User endpoint to update a review comment on a DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_team_dar_application_review_request import CreateTeamDarApplicationReviewRequest
from gateway_api_sdk.models.update_team_dar_application_question_review200_response import UpdateTeamDarApplicationQuestionReview200Response
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
    api_instance = gateway_api_sdk.DataAccessApplicationReviewApi(api_client)
    user_id = 1 # int | User id
    id = 1 # int | DAR application id
    review_id = 1 # int | DAR application review id
    create_team_dar_application_review_request = gateway_api_sdk.CreateTeamDarApplicationReviewRequest() # CreateTeamDarApplicationReviewRequest | DataAccessApplicationReview definition

    try:
        # DataAccessApplicationReview@userUpdateGlobal
        api_response = api_instance.update_user_dar_application_review(user_id, id, review_id, create_team_dar_application_review_request)
        print("The response of DataAccessApplicationReviewApi->update_user_dar_application_review:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationReviewApi->update_user_dar_application_review: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| User id | 
 **id** | **int**| DAR application id | 
 **review_id** | **int**| DAR application review id | 
 **create_team_dar_application_review_request** | [**CreateTeamDarApplicationReviewRequest**](CreateTeamDarApplicationReviewRequest.md)| DataAccessApplicationReview definition | 

### Return type

[**UpdateTeamDarApplicationQuestionReview200Response**](UpdateTeamDarApplicationQuestionReview200Response.md)

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

