# gateway_api_sdk.QuestionBankApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**a3f9ce42420fdef136cfc7b0de8e2683**](QuestionBankApi.md#a3f9ce42420fdef136cfc7b0de8e2683) | **GET** /api/v1/questions/version/{id} | QuestionBank@showVersion
[**call_04e09f4aada3406dbc08715865880f4f**](QuestionBankApi.md#call_04e09f4aada3406dbc08715865880f4f) | **GET** /api/v1/teams/{teamId}/questions/section/{sectionId} | TeamQuestionBank@indexBySection
[**call_17336ba551813e00975d3c2da09211c0**](QuestionBankApi.md#call_17336ba551813e00975d3c2da09211c0) | **GET** /api/v1/questions/{id} | QuestionBank@show
[**call_35856fcdf6980ae4da3303ec5a8d90b7**](QuestionBankApi.md#call_35856fcdf6980ae4da3303ec5a8d90b7) | **GET** /api/v1/questions | QuestionBank@index
[**call_35b36a3a067579d62500b09623dbffb6**](QuestionBankApi.md#call_35b36a3a067579d62500b09623dbffb6) | **GET** /api/v1/questions/{id}/files/{fileId} | QuestionBank@destroyFile
[**call_38b0b31c2029a219013fa640588a4a69**](QuestionBankApi.md#call_38b0b31c2029a219013fa640588a4a69) | **POST** /api/v1/questions | QuestionBank@store
[**call_64d6f1d6c88cbcfccd3e511b29c394d6**](QuestionBankApi.md#call_64d6f1d6c88cbcfccd3e511b29c394d6) | **PUT** /api/v1/questions/{id} | QuestionBank@update
[**d38b27b30f91d05932ca855e021c8ffd**](QuestionBankApi.md#d38b27b30f91d05932ca855e021c8ffd) | **PATCH** /api/v1/questions/{id} | QuestionBank@update
[**da82f7ce4870bd37af28a192877b22a7**](QuestionBankApi.md#da82f7ce4870bd37af28a192877b22a7) | **PATCH** /api/v1/questions/{id}/{status} | QuestionBank@updateStatus
[**dbaa6922ceaa314314605cba51dbb9df**](QuestionBankApi.md#dbaa6922ceaa314314605cba51dbb9df) | **GET** /api/v1/questions/archived | QuestionBank@indexArchived
[**e7408526aeb9ed9cc633d4a9f25cfa14**](QuestionBankApi.md#e7408526aeb9ed9cc633d4a9f25cfa14) | **DELETE** /api/v1/questions/{id} | QuestionBank@destroy
[**ea6f671b0436fa57891fe098994556a1**](QuestionBankApi.md#ea6f671b0436fa57891fe098994556a1) | **GET** /api/v1/questions/standard | QuestionBank@indexStandard
[**fa7079be66c6e1f5a236ecac24b63e2b**](QuestionBankApi.md#fa7079be66c6e1f5a236ecac24b63e2b) | **GET** /api/v1/questions/custom | QuestionBank@indexCustom


# **a3f9ce42420fdef136cfc7b0de8e2683**
> A3f9ce42420fdef136cfc7b0de8e2683200Response a3f9ce42420fdef136cfc7b0de8e2683(id)

QuestionBank@showVersion

Return a single system question bank question version

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.a3f9ce42420fdef136cfc7b0de8e2683200_response import A3f9ce42420fdef136cfc7b0de8e2683200Response
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
        api_response = api_instance.a3f9ce42420fdef136cfc7b0de8e2683(id)
        print("The response of QuestionBankApi->a3f9ce42420fdef136cfc7b0de8e2683:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuestionBankApi->a3f9ce42420fdef136cfc7b0de8e2683: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| question bank question version id | 

### Return type

[**A3f9ce42420fdef136cfc7b0de8e2683200Response**](A3f9ce42420fdef136cfc7b0de8e2683200Response.md)

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

# **call_04e09f4aada3406dbc08715865880f4f**
> Model04e09f4aada3406dbc08715865880f4f200Response call_04e09f4aada3406dbc08715865880f4f(team_id, section_id, is_child=is_child)

TeamQuestionBank@indexBySection

List of question bank questions by section

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model04e09f4aada3406dbc08715865880f4f200_response import Model04e09f4aada3406dbc08715865880f4f200Response
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
        api_response = api_instance.call_04e09f4aada3406dbc08715865880f4f(team_id, section_id, is_child=is_child)
        print("The response of QuestionBankApi->call_04e09f4aada3406dbc08715865880f4f:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuestionBankApi->call_04e09f4aada3406dbc08715865880f4f: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team ID | 
 **section_id** | **int**| section id | 
 **is_child** | **int**| filter on is_child field | [optional] 

### Return type

[**Model04e09f4aada3406dbc08715865880f4f200Response**](Model04e09f4aada3406dbc08715865880f4f200Response.md)

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

# **call_17336ba551813e00975d3c2da09211c0**
> Model17336ba551813e00975d3c2da09211c0200Response call_17336ba551813e00975d3c2da09211c0(id)

QuestionBank@show

Return the latest question bank question version for the supplied question id, in an FE-friendly format

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model17336ba551813e00975d3c2da09211c0200_response import Model17336ba551813e00975d3c2da09211c0200Response
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
        api_response = api_instance.call_17336ba551813e00975d3c2da09211c0(id)
        print("The response of QuestionBankApi->call_17336ba551813e00975d3c2da09211c0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuestionBankApi->call_17336ba551813e00975d3c2da09211c0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| question bank question id | 

### Return type

[**Model17336ba551813e00975d3c2da09211c0200Response**](Model17336ba551813e00975d3c2da09211c0200Response.md)

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

# **call_35856fcdf6980ae4da3303ec5a8d90b7**
> Model35856fcdf6980ae4da3303ec5a8d90b7200Response call_35856fcdf6980ae4da3303ec5a8d90b7(section_id=section_id, is_child=is_child, per_page=per_page, page=page)

QuestionBank@index

List of question bank questions

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model35856fcdf6980ae4da3303ec5a8d90b7200_response import Model35856fcdf6980ae4da3303ec5a8d90b7200Response
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
        api_response = api_instance.call_35856fcdf6980ae4da3303ec5a8d90b7(section_id=section_id, is_child=is_child, per_page=per_page, page=page)
        print("The response of QuestionBankApi->call_35856fcdf6980ae4da3303ec5a8d90b7:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuestionBankApi->call_35856fcdf6980ae4da3303ec5a8d90b7: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **section_id** | **int**| section id | [optional] 
 **is_child** | **int**| filter on is_child field | [optional] 
 **per_page** | **int**| per page | [optional] 
 **page** | **int**| page | [optional] 

### Return type

[**Model35856fcdf6980ae4da3303ec5a8d90b7200Response**](Model35856fcdf6980ae4da3303ec5a8d90b7200Response.md)

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

# **call_35b36a3a067579d62500b09623dbffb6**
> C29b5b3424f7317b69b4bda048ccfafb200Response call_35b36a3a067579d62500b09623dbffb6(id, file_id)

QuestionBank@destroyFile

Download a system question bank question

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
    api_instance = gateway_api_sdk.QuestionBankApi(api_client)
    id = 1 # int | question bank question id
    file_id = 1 # int | file uuid

    try:
        # QuestionBank@destroyFile
        api_response = api_instance.call_35b36a3a067579d62500b09623dbffb6(id, file_id)
        print("The response of QuestionBankApi->call_35b36a3a067579d62500b09623dbffb6:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuestionBankApi->call_35b36a3a067579d62500b09623dbffb6: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| question bank question id | 
 **file_id** | **int**| file uuid | 

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

# **call_38b0b31c2029a219013fa640588a4a69**
> Dd76b8d73b7ea8b4951f03d7c0904c92200Response call_38b0b31c2029a219013fa640588a4a69(model38b0b31c2029a219013fa640588a4a69_request)

QuestionBank@store

Create a new system question bank question with FE-helpful input format

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.dd76b8d73b7ea8b4951f03d7c0904c92200_response import Dd76b8d73b7ea8b4951f03d7c0904c92200Response
from gateway_api_sdk.models.model38b0b31c2029a219013fa640588a4a69_request import Model38b0b31c2029a219013fa640588a4a69Request
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
    model38b0b31c2029a219013fa640588a4a69_request = gateway_api_sdk.Model38b0b31c2029a219013fa640588a4a69Request() # Model38b0b31c2029a219013fa640588a4a69Request | QuestionBank definition

    try:
        # QuestionBank@store
        api_response = api_instance.call_38b0b31c2029a219013fa640588a4a69(model38b0b31c2029a219013fa640588a4a69_request)
        print("The response of QuestionBankApi->call_38b0b31c2029a219013fa640588a4a69:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuestionBankApi->call_38b0b31c2029a219013fa640588a4a69: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **model38b0b31c2029a219013fa640588a4a69_request** | [**Model38b0b31c2029a219013fa640588a4a69Request**](Model38b0b31c2029a219013fa640588a4a69Request.md)| QuestionBank definition | 

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
**200** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **call_64d6f1d6c88cbcfccd3e511b29c394d6**
> Model64d6f1d6c88cbcfccd3e511b29c394d6200Response call_64d6f1d6c88cbcfccd3e511b29c394d6(id, model64d6f1d6c88cbcfccd3e511b29c394d6_request)

QuestionBank@update

Update a system question bank question - children and their versions are updated through parents

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model64d6f1d6c88cbcfccd3e511b29c394d6200_response import Model64d6f1d6c88cbcfccd3e511b29c394d6200Response
from gateway_api_sdk.models.model64d6f1d6c88cbcfccd3e511b29c394d6_request import Model64d6f1d6c88cbcfccd3e511b29c394d6Request
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
    model64d6f1d6c88cbcfccd3e511b29c394d6_request = gateway_api_sdk.Model64d6f1d6c88cbcfccd3e511b29c394d6Request() # Model64d6f1d6c88cbcfccd3e511b29c394d6Request | QuestionBank definition

    try:
        # QuestionBank@update
        api_response = api_instance.call_64d6f1d6c88cbcfccd3e511b29c394d6(id, model64d6f1d6c88cbcfccd3e511b29c394d6_request)
        print("The response of QuestionBankApi->call_64d6f1d6c88cbcfccd3e511b29c394d6:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuestionBankApi->call_64d6f1d6c88cbcfccd3e511b29c394d6: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| question bank question id | 
 **model64d6f1d6c88cbcfccd3e511b29c394d6_request** | [**Model64d6f1d6c88cbcfccd3e511b29c394d6Request**](Model64d6f1d6c88cbcfccd3e511b29c394d6Request.md)| QuestionBank definition | 

### Return type

[**Model64d6f1d6c88cbcfccd3e511b29c394d6200Response**](Model64d6f1d6c88cbcfccd3e511b29c394d6200Response.md)

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

# **d38b27b30f91d05932ca855e021c8ffd**
> Model64d6f1d6c88cbcfccd3e511b29c394d6200Response d38b27b30f91d05932ca855e021c8ffd(id, d38b27b30f91d05932ca855e021c8ffd_request)

QuestionBank@update

Edit a system question bank question - use this for parents and children separately

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.d38b27b30f91d05932ca855e021c8ffd_request import D38b27b30f91d05932ca855e021c8ffdRequest
from gateway_api_sdk.models.model64d6f1d6c88cbcfccd3e511b29c394d6200_response import Model64d6f1d6c88cbcfccd3e511b29c394d6200Response
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
    d38b27b30f91d05932ca855e021c8ffd_request = gateway_api_sdk.D38b27b30f91d05932ca855e021c8ffdRequest() # D38b27b30f91d05932ca855e021c8ffdRequest | QuestionBank definition

    try:
        # QuestionBank@update
        api_response = api_instance.d38b27b30f91d05932ca855e021c8ffd(id, d38b27b30f91d05932ca855e021c8ffd_request)
        print("The response of QuestionBankApi->d38b27b30f91d05932ca855e021c8ffd:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuestionBankApi->d38b27b30f91d05932ca855e021c8ffd: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| question bank question id | 
 **d38b27b30f91d05932ca855e021c8ffd_request** | [**D38b27b30f91d05932ca855e021c8ffdRequest**](D38b27b30f91d05932ca855e021c8ffdRequest.md)| QuestionBank definition | 

### Return type

[**Model64d6f1d6c88cbcfccd3e511b29c394d6200Response**](Model64d6f1d6c88cbcfccd3e511b29c394d6200Response.md)

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

# **da82f7ce4870bd37af28a192877b22a7**
> Da82f7ce4870bd37af28a192877b22a7200Response da82f7ce4870bd37af28a192877b22a7(id, status)

QuestionBank@updateStatus

Lock, unlock, archive or unarchive a question bank question

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.da82f7ce4870bd37af28a192877b22a7200_response import Da82f7ce4870bd37af28a192877b22a7200Response
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
        api_response = api_instance.da82f7ce4870bd37af28a192877b22a7(id, status)
        print("The response of QuestionBankApi->da82f7ce4870bd37af28a192877b22a7:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuestionBankApi->da82f7ce4870bd37af28a192877b22a7: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| question bank question id | 
 **status** | **str**| lock or unlock | 

### Return type

[**Da82f7ce4870bd37af28a192877b22a7200Response**](Da82f7ce4870bd37af28a192877b22a7200Response.md)

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

# **dbaa6922ceaa314314605cba51dbb9df**
> Model35856fcdf6980ae4da3303ec5a8d90b7200Response dbaa6922ceaa314314605cba51dbb9df(section_id=section_id, is_child=is_child, per_page=per_page, page=page)

QuestionBank@indexArchived

List of archived question bank questions

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model35856fcdf6980ae4da3303ec5a8d90b7200_response import Model35856fcdf6980ae4da3303ec5a8d90b7200Response
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
        api_response = api_instance.dbaa6922ceaa314314605cba51dbb9df(section_id=section_id, is_child=is_child, per_page=per_page, page=page)
        print("The response of QuestionBankApi->dbaa6922ceaa314314605cba51dbb9df:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuestionBankApi->dbaa6922ceaa314314605cba51dbb9df: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **section_id** | **int**| section id | [optional] 
 **is_child** | **int**| filter on is_child field | [optional] 
 **per_page** | **int**| per page | [optional] 
 **page** | **int**| page | [optional] 

### Return type

[**Model35856fcdf6980ae4da3303ec5a8d90b7200Response**](Model35856fcdf6980ae4da3303ec5a8d90b7200Response.md)

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

# **e7408526aeb9ed9cc633d4a9f25cfa14**
> C29b5b3424f7317b69b4bda048ccfafb200Response e7408526aeb9ed9cc633d4a9f25cfa14(id)

QuestionBank@destroy

Delete a system question bank question

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
    api_instance = gateway_api_sdk.QuestionBankApi(api_client)
    id = 1 # int | question bank question id

    try:
        # QuestionBank@destroy
        api_response = api_instance.e7408526aeb9ed9cc633d4a9f25cfa14(id)
        print("The response of QuestionBankApi->e7408526aeb9ed9cc633d4a9f25cfa14:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuestionBankApi->e7408526aeb9ed9cc633d4a9f25cfa14: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| question bank question id | 

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

# **ea6f671b0436fa57891fe098994556a1**
> Ea6f671b0436fa57891fe098994556a1200Response ea6f671b0436fa57891fe098994556a1(section_id=section_id, is_child=is_child, per_page=per_page, page=page)

QuestionBank@indexStandard

List of standard question bank questions

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.ea6f671b0436fa57891fe098994556a1200_response import Ea6f671b0436fa57891fe098994556a1200Response
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
        api_response = api_instance.ea6f671b0436fa57891fe098994556a1(section_id=section_id, is_child=is_child, per_page=per_page, page=page)
        print("The response of QuestionBankApi->ea6f671b0436fa57891fe098994556a1:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuestionBankApi->ea6f671b0436fa57891fe098994556a1: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **section_id** | **int**| section id | [optional] 
 **is_child** | **int**| filter on is_child field | [optional] 
 **per_page** | **int**| per page | [optional] 
 **page** | **int**| page | [optional] 

### Return type

[**Ea6f671b0436fa57891fe098994556a1200Response**](Ea6f671b0436fa57891fe098994556a1200Response.md)

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

# **fa7079be66c6e1f5a236ecac24b63e2b**
> Fa7079be66c6e1f5a236ecac24b63e2b200Response fa7079be66c6e1f5a236ecac24b63e2b(section_id=section_id, is_child=is_child, per_page=per_page, page=page)

QuestionBank@indexCustom

List of custom question bank questions

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fa7079be66c6e1f5a236ecac24b63e2b200_response import Fa7079be66c6e1f5a236ecac24b63e2b200Response
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
        api_response = api_instance.fa7079be66c6e1f5a236ecac24b63e2b(section_id=section_id, is_child=is_child, per_page=per_page, page=page)
        print("The response of QuestionBankApi->fa7079be66c6e1f5a236ecac24b63e2b:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuestionBankApi->fa7079be66c6e1f5a236ecac24b63e2b: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **section_id** | **int**| section id | [optional] 
 **is_child** | **int**| filter on is_child field | [optional] 
 **per_page** | **int**| per page | [optional] 
 **page** | **int**| page | [optional] 

### Return type

[**Fa7079be66c6e1f5a236ecac24b63e2b200Response**](Fa7079be66c6e1f5a236ecac24b63e2b200Response.md)

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

