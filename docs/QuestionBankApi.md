# gateway_api_sdk.QuestionBankApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_question_bank_question**](QuestionBankApi.md#create_question_bank_question) | **POST** /api/v1/questions | QuestionBank@store
[**delete_question_bank_question**](QuestionBankApi.md#delete_question_bank_question) | **DELETE** /api/v1/questions/{id} | QuestionBank@destroy
[**download_question_bank_question_file**](QuestionBankApi.md#download_question_bank_question_file) | **GET** /api/v1/questions/{id}/files/{fileId} | QuestionBank@destroyFile
[**edit_question_bank_question**](QuestionBankApi.md#edit_question_bank_question) | **PATCH** /api/v1/questions/{id} | QuestionBank@update
[**fetch_archived_question_bank_questions**](QuestionBankApi.md#fetch_archived_question_bank_questions) | **GET** /api/v1/questions/archived | QuestionBank@indexArchived
[**fetch_custom_question_bank_questions**](QuestionBankApi.md#fetch_custom_question_bank_questions) | **GET** /api/v1/questions/custom | QuestionBank@indexCustom
[**fetch_question_bank_question**](QuestionBankApi.md#fetch_question_bank_question) | **GET** /api/v1/questions/{id} | QuestionBank@show
[**fetch_question_bank_question_version**](QuestionBankApi.md#fetch_question_bank_question_version) | **GET** /api/v1/questions/version/{id} | QuestionBank@showVersion
[**fetch_question_bank_questions**](QuestionBankApi.md#fetch_question_bank_questions) | **GET** /api/v1/questions | QuestionBank@index
[**fetch_standard_question_bank_questions**](QuestionBankApi.md#fetch_standard_question_bank_questions) | **GET** /api/v1/questions/standard | QuestionBank@indexStandard
[**fetch_team_question_bank_questions_by_section**](QuestionBankApi.md#fetch_team_question_bank_questions_by_section) | **GET** /api/v1/teams/{teamId}/questions/section/{sectionId} | TeamQuestionBank@indexBySection
[**update_question_bank_question**](QuestionBankApi.md#update_question_bank_question) | **PUT** /api/v1/questions/{id} | QuestionBank@update
[**update_question_bank_question_status**](QuestionBankApi.md#update_question_bank_question_status) | **PATCH** /api/v1/questions/{id}/{status} | QuestionBank@updateStatus


# **create_question_bank_question**
> CreateCategories200Response create_question_bank_question(create_question_bank_question_request)

QuestionBank@store

Create a new system question bank question with FE-helpful input format

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_categories200_response import CreateCategories200Response
from gateway_api_sdk.models.create_question_bank_question_request import CreateQuestionBankQuestionRequest
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
    api_instance = gateway_api_sdk.QuestionBankApi(api_client)
    create_question_bank_question_request = gateway_api_sdk.CreateQuestionBankQuestionRequest() # CreateQuestionBankQuestionRequest | QuestionBank definition

    try:
        # QuestionBank@store
        api_response = api_instance.create_question_bank_question(create_question_bank_question_request)
        print("The response of QuestionBankApi->create_question_bank_question:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuestionBankApi->create_question_bank_question: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_question_bank_question_request** | [**CreateQuestionBankQuestionRequest**](CreateQuestionBankQuestionRequest.md)| QuestionBank definition | 

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

# **delete_question_bank_question**
> DeleteAliases200Response delete_question_bank_question(id)

QuestionBank@destroy

Delete a system question bank question

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
    api_instance = gateway_api_sdk.QuestionBankApi(api_client)
    id = 1 # int | question bank question id

    try:
        # QuestionBank@destroy
        api_response = api_instance.delete_question_bank_question(id)
        print("The response of QuestionBankApi->delete_question_bank_question:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuestionBankApi->delete_question_bank_question: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| question bank question id | 

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

# **download_question_bank_question_file**
> DeleteAliases200Response download_question_bank_question_file(id, file_id)

QuestionBank@destroyFile

Download a system question bank question

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
    api_instance = gateway_api_sdk.QuestionBankApi(api_client)
    id = 1 # int | question bank question id
    file_id = 1 # int | file uuid

    try:
        # QuestionBank@destroyFile
        api_response = api_instance.download_question_bank_question_file(id, file_id)
        print("The response of QuestionBankApi->download_question_bank_question_file:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuestionBankApi->download_question_bank_question_file: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| question bank question id | 
 **file_id** | **int**| file uuid | 

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

# **edit_question_bank_question**
> UpdateQuestionBankQuestion200Response edit_question_bank_question(id, edit_question_bank_question_request)

QuestionBank@update

Edit a system question bank question - use this for parents and children separately

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.edit_question_bank_question_request import EditQuestionBankQuestionRequest
from gateway_api_sdk.models.update_question_bank_question200_response import UpdateQuestionBankQuestion200Response
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
    api_instance = gateway_api_sdk.QuestionBankApi(api_client)
    id = 1 # int | question bank question id
    edit_question_bank_question_request = gateway_api_sdk.EditQuestionBankQuestionRequest() # EditQuestionBankQuestionRequest | QuestionBank definition

    try:
        # QuestionBank@update
        api_response = api_instance.edit_question_bank_question(id, edit_question_bank_question_request)
        print("The response of QuestionBankApi->edit_question_bank_question:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuestionBankApi->edit_question_bank_question: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| question bank question id | 
 **edit_question_bank_question_request** | [**EditQuestionBankQuestionRequest**](EditQuestionBankQuestionRequest.md)| QuestionBank definition | 

### Return type

[**UpdateQuestionBankQuestion200Response**](UpdateQuestionBankQuestion200Response.md)

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

# **fetch_archived_question_bank_questions**
> FetchQuestionBankQuestions200Response fetch_archived_question_bank_questions(section_id=section_id, is_child=is_child, per_page=per_page, page=page)

QuestionBank@indexArchived

List of archived question bank questions

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_question_bank_questions200_response import FetchQuestionBankQuestions200Response
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
    api_instance = gateway_api_sdk.QuestionBankApi(api_client)
    section_id = 1 # int | section id (optional)
    is_child = 1 # int | filter on is_child field (optional)
    per_page = 1 # int | per page (optional)
    page = 1 # int | page (optional)

    try:
        # QuestionBank@indexArchived
        api_response = api_instance.fetch_archived_question_bank_questions(section_id=section_id, is_child=is_child, per_page=per_page, page=page)
        print("The response of QuestionBankApi->fetch_archived_question_bank_questions:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuestionBankApi->fetch_archived_question_bank_questions: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **section_id** | **int**| section id | [optional] 
 **is_child** | **int**| filter on is_child field | [optional] 
 **per_page** | **int**| per page | [optional] 
 **page** | **int**| page | [optional] 

### Return type

[**FetchQuestionBankQuestions200Response**](FetchQuestionBankQuestions200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_custom_question_bank_questions**
> FetchCustomQuestionBankQuestions200Response fetch_custom_question_bank_questions(section_id=section_id, is_child=is_child, per_page=per_page, page=page)

QuestionBank@indexCustom

List of custom question bank questions

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_custom_question_bank_questions200_response import FetchCustomQuestionBankQuestions200Response
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
    api_instance = gateway_api_sdk.QuestionBankApi(api_client)
    section_id = 1 # int | section id (optional)
    is_child = 1 # int | filter on is_child field (optional)
    per_page = 1 # int | per page (optional)
    page = 1 # int | page (optional)

    try:
        # QuestionBank@indexCustom
        api_response = api_instance.fetch_custom_question_bank_questions(section_id=section_id, is_child=is_child, per_page=per_page, page=page)
        print("The response of QuestionBankApi->fetch_custom_question_bank_questions:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuestionBankApi->fetch_custom_question_bank_questions: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **section_id** | **int**| section id | [optional] 
 **is_child** | **int**| filter on is_child field | [optional] 
 **per_page** | **int**| per page | [optional] 
 **page** | **int**| page | [optional] 

### Return type

[**FetchCustomQuestionBankQuestions200Response**](FetchCustomQuestionBankQuestions200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_question_bank_question**
> FetchQuestionBankQuestion200Response fetch_question_bank_question(id)

QuestionBank@show

Return the latest question bank question version for the supplied question id, in an FE-friendly format

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_question_bank_question200_response import FetchQuestionBankQuestion200Response
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
    api_instance = gateway_api_sdk.QuestionBankApi(api_client)
    id = 1 # int | question bank question id

    try:
        # QuestionBank@show
        api_response = api_instance.fetch_question_bank_question(id)
        print("The response of QuestionBankApi->fetch_question_bank_question:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuestionBankApi->fetch_question_bank_question: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| question bank question id | 

### Return type

[**FetchQuestionBankQuestion200Response**](FetchQuestionBankQuestion200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_question_bank_question_version**
> FetchQuestionBankQuestionVersion200Response fetch_question_bank_question_version(id)

QuestionBank@showVersion

Return a single system question bank question version

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_question_bank_question_version200_response import FetchQuestionBankQuestionVersion200Response
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
    api_instance = gateway_api_sdk.QuestionBankApi(api_client)
    id = 1 # int | question bank question version id

    try:
        # QuestionBank@showVersion
        api_response = api_instance.fetch_question_bank_question_version(id)
        print("The response of QuestionBankApi->fetch_question_bank_question_version:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuestionBankApi->fetch_question_bank_question_version: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| question bank question version id | 

### Return type

[**FetchQuestionBankQuestionVersion200Response**](FetchQuestionBankQuestionVersion200Response.md)

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

# **fetch_question_bank_questions**
> FetchQuestionBankQuestions200Response fetch_question_bank_questions(section_id=section_id, is_child=is_child, per_page=per_page, page=page)

QuestionBank@index

List of question bank questions

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_question_bank_questions200_response import FetchQuestionBankQuestions200Response
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
    api_instance = gateway_api_sdk.QuestionBankApi(api_client)
    section_id = 1 # int | section id (optional)
    is_child = 1 # int | filter on is_child field (optional)
    per_page = 1 # int | per page (optional)
    page = 1 # int | page (optional)

    try:
        # QuestionBank@index
        api_response = api_instance.fetch_question_bank_questions(section_id=section_id, is_child=is_child, per_page=per_page, page=page)
        print("The response of QuestionBankApi->fetch_question_bank_questions:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuestionBankApi->fetch_question_bank_questions: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **section_id** | **int**| section id | [optional] 
 **is_child** | **int**| filter on is_child field | [optional] 
 **per_page** | **int**| per page | [optional] 
 **page** | **int**| page | [optional] 

### Return type

[**FetchQuestionBankQuestions200Response**](FetchQuestionBankQuestions200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_standard_question_bank_questions**
> FetchStandardQuestionBankQuestions200Response fetch_standard_question_bank_questions(section_id=section_id, is_child=is_child, per_page=per_page, page=page)

QuestionBank@indexStandard

List of standard question bank questions

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_standard_question_bank_questions200_response import FetchStandardQuestionBankQuestions200Response
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
    api_instance = gateway_api_sdk.QuestionBankApi(api_client)
    section_id = 1 # int | section id (optional)
    is_child = 1 # int | filter on is_child field (optional)
    per_page = 1 # int | per page (optional)
    page = 1 # int | page (optional)

    try:
        # QuestionBank@indexStandard
        api_response = api_instance.fetch_standard_question_bank_questions(section_id=section_id, is_child=is_child, per_page=per_page, page=page)
        print("The response of QuestionBankApi->fetch_standard_question_bank_questions:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuestionBankApi->fetch_standard_question_bank_questions: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **section_id** | **int**| section id | [optional] 
 **is_child** | **int**| filter on is_child field | [optional] 
 **per_page** | **int**| per page | [optional] 
 **page** | **int**| page | [optional] 

### Return type

[**FetchStandardQuestionBankQuestions200Response**](FetchStandardQuestionBankQuestions200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_team_question_bank_questions_by_section**
> FetchTeamQuestionBankQuestionsBySection200Response fetch_team_question_bank_questions_by_section(team_id, section_id, is_child=is_child)

TeamQuestionBank@indexBySection

List of question bank questions by section

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_team_question_bank_questions_by_section200_response import FetchTeamQuestionBankQuestionsBySection200Response
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
    api_instance = gateway_api_sdk.QuestionBankApi(api_client)
    team_id = 1 # int | Team ID
    section_id = 1 # int | section id
    is_child = 1 # int | filter on is_child field (optional)

    try:
        # TeamQuestionBank@indexBySection
        api_response = api_instance.fetch_team_question_bank_questions_by_section(team_id, section_id, is_child=is_child)
        print("The response of QuestionBankApi->fetch_team_question_bank_questions_by_section:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuestionBankApi->fetch_team_question_bank_questions_by_section: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team ID | 
 **section_id** | **int**| section id | 
 **is_child** | **int**| filter on is_child field | [optional] 

### Return type

[**FetchTeamQuestionBankQuestionsBySection200Response**](FetchTeamQuestionBankQuestionsBySection200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_question_bank_question**
> UpdateQuestionBankQuestion200Response update_question_bank_question(id, update_question_bank_question_request)

QuestionBank@update

Update a system question bank question - children and their versions are updated through parents

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.update_question_bank_question200_response import UpdateQuestionBankQuestion200Response
from gateway_api_sdk.models.update_question_bank_question_request import UpdateQuestionBankQuestionRequest
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
    api_instance = gateway_api_sdk.QuestionBankApi(api_client)
    id = 1 # int | question bank question id
    update_question_bank_question_request = gateway_api_sdk.UpdateQuestionBankQuestionRequest() # UpdateQuestionBankQuestionRequest | QuestionBank definition

    try:
        # QuestionBank@update
        api_response = api_instance.update_question_bank_question(id, update_question_bank_question_request)
        print("The response of QuestionBankApi->update_question_bank_question:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuestionBankApi->update_question_bank_question: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| question bank question id | 
 **update_question_bank_question_request** | [**UpdateQuestionBankQuestionRequest**](UpdateQuestionBankQuestionRequest.md)| QuestionBank definition | 

### Return type

[**UpdateQuestionBankQuestion200Response**](UpdateQuestionBankQuestion200Response.md)

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

# **update_question_bank_question_status**
> UpdateQuestionBankQuestionStatus200Response update_question_bank_question_status(id, status)

QuestionBank@updateStatus

Lock, unlock, archive or unarchive a question bank question

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.update_question_bank_question_status200_response import UpdateQuestionBankQuestionStatus200Response
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
    api_instance = gateway_api_sdk.QuestionBankApi(api_client)
    id = 1 # int | question bank question id
    status = 'lock' # str | lock or unlock

    try:
        # QuestionBank@updateStatus
        api_response = api_instance.update_question_bank_question_status(id, status)
        print("The response of QuestionBankApi->update_question_bank_question_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuestionBankApi->update_question_bank_question_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| question bank question id | 
 **status** | **str**| lock or unlock | 

### Return type

[**UpdateQuestionBankQuestionStatus200Response**](UpdateQuestionBankQuestionStatus200Response.md)

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

