# gateway_api_sdk.DatasetsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_team_unique_fields_datasets_v2**](DatasetsApi.md#count_team_unique_fields_datasets_v2) | **GET** /api/v2/teams/{teamId}/datasets/count/{field} | TeamDatasetController@count
[**count_unique_fields**](DatasetsApi.md#count_unique_fields) | **GET** /api/v1/datasets/count/{field} | DatasetController@count
[**create_datasets**](DatasetsApi.md#create_datasets) | **POST** /api/v1/datasets | DatasetController@store
[**create_datasets_integrations**](DatasetsApi.md#create_datasets_integrations) | **POST** /api/v1/integrations/datasets | IntegrationDatasetController@store
[**create_datasets_linkage_extraction**](DatasetsApi.md#create_datasets_linkage_extraction) | **POST** /api/v1/datasets/admin_ctrl/trigger/linkage_extraction | Trigger Term Extraction for Datasets
[**create_datasets_term_extraction**](DatasetsApi.md#create_datasets_term_extraction) | **POST** /api/v1/datasets/admin_ctrl/trigger/term_extraction | Trigger Term Extraction for Datasets
[**create_datasets_v2**](DatasetsApi.md#create_datasets_v2) | **POST** /api/v2/datasets | DatasetController@store
[**create_team_datasets_v2**](DatasetsApi.md#create_team_datasets_v2) | **POST** /api/v2/teams/{teamId}/datasets | TeamDatasetController@store
[**delete_datasets**](DatasetsApi.md#delete_datasets) | **DELETE** /api/v1/datasets/{id} | DatasetController@destroy
[**delete_datasets_integrations**](DatasetsApi.md#delete_datasets_integrations) | **DELETE** /api/v1/integrations/datasets/{id} | IntegrationDatasetController@destroy
[**delete_datasets_v2**](DatasetsApi.md#delete_datasets_v2) | **DELETE** /api/v2/datasets/{id} | Delete a dataset
[**delete_team_datasets_v2**](DatasetsApi.md#delete_team_datasets_v2) | **DELETE** /api/v2/teams/{teamId}/datasets/{id} | TeamDatasetController@destroy
[**export_dataset_metadata**](DatasetsApi.md#export_dataset_metadata) | **GET** /api/v1/datasets/export_metadata/{id} | DatasetController@exportMetadata
[**export_datasets**](DatasetsApi.md#export_datasets) | **GET** /api/v1/datasets/export | DatasetController@export
[**export_dur**](DatasetsApi.md#export_dur) | **GET** /api/v1/dur/export | DurController@export
[**export_mock_dataset**](DatasetsApi.md#export_mock_dataset) | **GET** /api/v1/datasets/export/mock | DatasetController@exportMock
[**export_mock_dataset_v2**](DatasetsApi.md#export_mock_dataset_v2) | **GET** /api/v2/datasets/export/mock | DatasetController@exportMock
[**fetch_all_datasets**](DatasetsApi.md#fetch_all_datasets) | **GET** /api/v1/datasets | DatasetController@index
[**fetch_all_datasets_integrations**](DatasetsApi.md#fetch_all_datasets_integrations) | **GET** /api/v1/integrations/datasets | IntegrationDatasetController@index
[**fetch_all_datasets_v2**](DatasetsApi.md#fetch_all_datasets_v2) | **GET** /api/v2/datasets | DatasetController@index
[**fetch_datasets**](DatasetsApi.md#fetch_datasets) | **GET** /api/v1/datasets/{id} | DatasetController@show
[**fetch_datasets_integrations**](DatasetsApi.md#fetch_datasets_integrations) | **GET** /api/v1/integrations/datasets/{id} | IntegrationDatasetController@show
[**fetch_datasets_v2**](DatasetsApi.md#fetch_datasets_v2) | **GET** /api/v2/datasets/{id} | DatasetController@showActive
[**fetch_team_datasets_status**](DatasetsApi.md#fetch_team_datasets_status) | **GET** /api/v2/teams/{teamId}/datasets/status/{status} | TeamDatasetController@indexStatus
[**fetch_team_datasets_v2**](DatasetsApi.md#fetch_team_datasets_v2) | **GET** /api/v2/teams/{teamId}/datasets/{id} | TeamDatasetController@show
[**patch_datasets**](DatasetsApi.md#patch_datasets) | **PATCH** /api/v1/datasets/{id} | DatasetController@edit
[**patch_datasets_integrations**](DatasetsApi.md#patch_datasets_integrations) | **PATCH** /api/v1/integrations/datasets/{id} | IntegrationDatasetController@edit
[**patch_datasets_v2**](DatasetsApi.md#patch_datasets_v2) | **PATCH** /api/v2/datasets/{id} | DatasetController@edit
[**patch_team_datasets_v2**](DatasetsApi.md#patch_team_datasets_v2) | **PATCH** /api/v2/teams/{teamId}/datasets/{id} | TeamDatasetController@edit
[**update_datasets**](DatasetsApi.md#update_datasets) | **PUT** /api/v1/datasets/{id} | DatasetController@update
[**update_datasets_integrations**](DatasetsApi.md#update_datasets_integrations) | **PUT** /api/v1/integrations/datasets/{id} | IntegrationDatasetController@update
[**update_datasets_v2**](DatasetsApi.md#update_datasets_v2) | **PUT** /api/v2/datasets/{id} | DatasetController@update
[**update_team_datasets_v2**](DatasetsApi.md#update_team_datasets_v2) | **PUT** /api/v2/teams/{teamId}/datasets/{id} | TeamDatasetController@update


# **count_team_unique_fields_datasets_v2**
> CountUniqueFieldsCollections200Response count_team_unique_fields_datasets_v2(team_id, var_field)

TeamDatasetController@count

Get team counts for distinct entries of a field in the model

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.count_unique_fields_collections200_response import CountUniqueFieldsCollections200Response
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
    api_instance = gateway_api_sdk.DatasetsApi(api_client)
    team_id = 1 # int | team id
    var_field = 'status' # str | name of the field to perform a count on

    try:
        # TeamDatasetController@count
        api_response = api_instance.count_team_unique_fields_datasets_v2(team_id, var_field)
        print("The response of DatasetsApi->count_team_unique_fields_datasets_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetsApi->count_team_unique_fields_datasets_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **var_field** | **str**| name of the field to perform a count on | 

### Return type

[**CountUniqueFieldsCollections200Response**](CountUniqueFieldsCollections200Response.md)

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

# **count_unique_fields**
> CountUniqueFieldsCollections200Response count_unique_fields(var_field, team_id)

DatasetController@count

Get Counts for distinct entries of a field in the model

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.count_unique_fields_collections200_response import CountUniqueFieldsCollections200Response
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
    api_instance = gateway_api_sdk.DatasetsApi(api_client)
    var_field = 'status' # str | name of the field to perform a count on
    team_id = 1 # int | team id

    try:
        # DatasetController@count
        api_response = api_instance.count_unique_fields(var_field, team_id)
        print("The response of DatasetsApi->count_unique_fields:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetsApi->count_unique_fields: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **var_field** | **str**| name of the field to perform a count on | 
 **team_id** | **int**| team id | 

### Return type

[**CountUniqueFieldsCollections200Response**](CountUniqueFieldsCollections200Response.md)

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

# **create_datasets**
> CreateCategories200Response create_datasets(create_datasets_request)

DatasetController@store

Create a new dataset

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_categories200_response import CreateCategories200Response
from gateway_api_sdk.models.create_datasets_request import CreateDatasetsRequest
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
    api_instance = gateway_api_sdk.DatasetsApi(api_client)
    create_datasets_request = gateway_api_sdk.CreateDatasetsRequest() # CreateDatasetsRequest | Pass user credentials

    try:
        # DatasetController@store
        api_response = api_instance.create_datasets(create_datasets_request)
        print("The response of DatasetsApi->create_datasets:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetsApi->create_datasets: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_datasets_request** | [**CreateDatasetsRequest**](CreateDatasetsRequest.md)| Pass user credentials | 

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
**201** | Created |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_datasets_integrations**
> CreateCategories200Response create_datasets_integrations(datasets_test_request, input_schema=input_schema, input_version=input_version)

IntegrationDatasetController@store

Create a new dataset

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_categories200_response import CreateCategories200Response
from gateway_api_sdk.models.datasets_test_request import DatasetsTestRequest
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
    api_instance = gateway_api_sdk.DatasetsApi(api_client)
    datasets_test_request = gateway_api_sdk.DatasetsTestRequest() # DatasetsTestRequest | Pass user credentials
    input_schema = 'HDRUK' # str | Input schema model. (optional)
    input_version = '3.0.0' # str | Input schema version. (optional)

    try:
        # IntegrationDatasetController@store
        api_response = api_instance.create_datasets_integrations(datasets_test_request, input_schema=input_schema, input_version=input_version)
        print("The response of DatasetsApi->create_datasets_integrations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetsApi->create_datasets_integrations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **datasets_test_request** | [**DatasetsTestRequest**](DatasetsTestRequest.md)| Pass user credentials | 
 **input_schema** | **str**| Input schema model. | [optional] 
 **input_version** | **str**| Input schema version. | [optional] 

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
**201** | Created |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_datasets_linkage_extraction**
> CreateDatasetsLinkageExtraction200Response create_datasets_linkage_extraction(authorization, create_datasets_linkage_extraction_request)

Trigger Term Extraction for Datasets

Triggers the term extraction job for datasets within a specified range and controls whether data is partially indexed in Elasticsearch.

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.create_datasets_linkage_extraction200_response import CreateDatasetsLinkageExtraction200Response
from gateway_api_sdk.models.create_datasets_linkage_extraction_request import CreateDatasetsLinkageExtractionRequest
from gateway_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = gateway_api_sdk.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with gateway_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = gateway_api_sdk.DatasetsApi(api_client)
    authorization = 'authorization_example' # str | JWT token for authorization in the format 'Bearer {token}'
    create_datasets_linkage_extraction_request = gateway_api_sdk.CreateDatasetsLinkageExtractionRequest() # CreateDatasetsLinkageExtractionRequest | 

    try:
        # Trigger Term Extraction for Datasets
        api_response = api_instance.create_datasets_linkage_extraction(authorization, create_datasets_linkage_extraction_request)
        print("The response of DatasetsApi->create_datasets_linkage_extraction:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetsApi->create_datasets_linkage_extraction: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **str**| JWT token for authorization in the format &#39;Bearer {token}&#39; | 
 **create_datasets_linkage_extraction_request** | [**CreateDatasetsLinkageExtractionRequest**](CreateDatasetsLinkageExtractionRequest.md)|  | 

### Return type

[**CreateDatasetsLinkageExtraction200Response**](CreateDatasetsLinkageExtraction200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Linkage extraction triggered successfully |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_datasets_term_extraction**
> CreateDatasetsTermExtraction200Response create_datasets_term_extraction(authorization, role, create_datasets_term_extraction_request)

Trigger Term Extraction for Datasets

Triggers the term extraction job for datasets within a specified range and controls whether data is partially indexed in Elasticsearch.

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.create_datasets_term_extraction200_response import CreateDatasetsTermExtraction200Response
from gateway_api_sdk.models.create_datasets_term_extraction_request import CreateDatasetsTermExtractionRequest
from gateway_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = gateway_api_sdk.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with gateway_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = gateway_api_sdk.DatasetsApi(api_client)
    authorization = 'authorization_example' # str | JWT token for authorization in the format 'Bearer {token}'
    role = 'role_example' # str | Role required to access this endpoint, e.g., 'hdruk.superadmin'
    create_datasets_term_extraction_request = gateway_api_sdk.CreateDatasetsTermExtractionRequest() # CreateDatasetsTermExtractionRequest | 

    try:
        # Trigger Term Extraction for Datasets
        api_response = api_instance.create_datasets_term_extraction(authorization, role, create_datasets_term_extraction_request)
        print("The response of DatasetsApi->create_datasets_term_extraction:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetsApi->create_datasets_term_extraction: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **str**| JWT token for authorization in the format &#39;Bearer {token}&#39; | 
 **role** | **str**| Role required to access this endpoint, e.g., &#39;hdruk.superadmin&#39; | 
 **create_datasets_term_extraction_request** | [**CreateDatasetsTermExtractionRequest**](CreateDatasetsTermExtractionRequest.md)|  | 

### Return type

[**CreateDatasetsTermExtraction200Response**](CreateDatasetsTermExtraction200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Term extraction triggered successfully |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_datasets_v2**
> CreateCategories200Response create_datasets_v2(create_datasets_v2_request)

DatasetController@store

Create a new dataset

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_categories200_response import CreateCategories200Response
from gateway_api_sdk.models.create_datasets_v2_request import CreateDatasetsV2Request
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
    api_instance = gateway_api_sdk.DatasetsApi(api_client)
    create_datasets_v2_request = gateway_api_sdk.CreateDatasetsV2Request() # CreateDatasetsV2Request | Pass user credentials

    try:
        # DatasetController@store
        api_response = api_instance.create_datasets_v2(create_datasets_v2_request)
        print("The response of DatasetsApi->create_datasets_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetsApi->create_datasets_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_datasets_v2_request** | [**CreateDatasetsV2Request**](CreateDatasetsV2Request.md)| Pass user credentials | 

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
**201** | Created |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_team_datasets_v2**
> CreateCategories200Response create_team_datasets_v2(team_id, create_team_datasets_v2_request)

TeamDatasetController@store

Create a new dataset for a team

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_categories200_response import CreateCategories200Response
from gateway_api_sdk.models.create_team_datasets_v2_request import CreateTeamDatasetsV2Request
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
    api_instance = gateway_api_sdk.DatasetsApi(api_client)
    team_id = 1 # int | team id
    create_team_datasets_v2_request = gateway_api_sdk.CreateTeamDatasetsV2Request() # CreateTeamDatasetsV2Request | Pass user credentials

    try:
        # TeamDatasetController@store
        api_response = api_instance.create_team_datasets_v2(team_id, create_team_datasets_v2_request)
        print("The response of DatasetsApi->create_team_datasets_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetsApi->create_team_datasets_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **create_team_datasets_v2_request** | [**CreateTeamDatasetsV2Request**](CreateTeamDatasetsV2Request.md)| Pass user credentials | 

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
**201** | Created |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_datasets**
> DeleteAliases200Response delete_datasets(id)

DatasetController@destroy

Delete a dataset

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
    api_instance = gateway_api_sdk.DatasetsApi(api_client)
    id = 1 # int | dataset id

    try:
        # DatasetController@destroy
        api_response = api_instance.delete_datasets(id)
        print("The response of DatasetsApi->delete_datasets:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetsApi->delete_datasets: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| dataset id | 

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

# **delete_datasets_integrations**
> DeleteAliases200Response delete_datasets_integrations(id)

IntegrationDatasetController@destroy

Delete a dataset

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
    api_instance = gateway_api_sdk.DatasetsApi(api_client)
    id = 1 # int | dataset id

    try:
        # IntegrationDatasetController@destroy
        api_response = api_instance.delete_datasets_integrations(id)
        print("The response of DatasetsApi->delete_datasets_integrations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetsApi->delete_datasets_integrations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| dataset id | 

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

# **delete_datasets_v2**
> DeleteAliases200Response delete_datasets_v2(id)

Delete a dataset

Delete a dataset

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
    api_instance = gateway_api_sdk.DatasetsApi(api_client)
    id = 1 # int | dataset id

    try:
        # Delete a dataset
        api_response = api_instance.delete_datasets_v2(id)
        print("The response of DatasetsApi->delete_datasets_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetsApi->delete_datasets_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| dataset id | 

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

# **delete_team_datasets_v2**
> DeleteAliases200Response delete_team_datasets_v2(team_id, id)

TeamDatasetController@destroy

Delete a team's dataset

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
    api_instance = gateway_api_sdk.DatasetsApi(api_client)
    team_id = 1 # int | team id
    id = 1 # int | dataset id

    try:
        # TeamDatasetController@destroy
        api_response = api_instance.delete_team_datasets_v2(team_id, id)
        print("The response of DatasetsApi->delete_team_datasets_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetsApi->delete_team_datasets_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **id** | **int**| dataset id | 

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

# **export_dataset_metadata**
> str export_dataset_metadata(id, download_type)

DatasetController@exportMetadata

Export Structural Metadata CSV of a single dataset

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
    api_instance = gateway_api_sdk.DatasetsApi(api_client)
    id = 1 # int | dataset id
    download_type = 'structural' # str | download type

    try:
        # DatasetController@exportMetadata
        api_response = api_instance.export_dataset_metadata(id, download_type)
        print("The response of DatasetsApi->export_dataset_metadata:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetsApi->export_dataset_metadata: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| dataset id | 
 **download_type** | **str**| download type | 

### Return type

**str**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/csv, application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | CSV file |  -  |
**400** | Bad request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **export_datasets**
> str export_datasets(team_id, dataset_id=dataset_id)

DatasetController@export

Export CSV Of All Datasets

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
    api_instance = gateway_api_sdk.DatasetsApi(api_client)
    team_id = 1 # int | team id
    dataset_id = 1 # int | dataset id (optional)

    try:
        # DatasetController@export
        api_response = api_instance.export_datasets(team_id, dataset_id=dataset_id)
        print("The response of DatasetsApi->export_datasets:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetsApi->export_datasets: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **dataset_id** | **int**| dataset id | [optional] 

### Return type

**str**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/csv, application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | CSV file |  -  |
**401** | Unauthorized |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **export_dur**
> str export_dur(team_id, dur_id=dur_id)

DurController@export

Export CSV Of All Dur's

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
    api_instance = gateway_api_sdk.DatasetsApi(api_client)
    team_id = 1 # int | team id
    dur_id = 1 # int | dur id (optional)

    try:
        # DurController@export
        api_response = api_instance.export_dur(team_id, dur_id=dur_id)
        print("The response of DatasetsApi->export_dur:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetsApi->export_dur: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **dur_id** | **int**| dur id | [optional] 

### Return type

**str**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/csv, application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | CSV file |  -  |
**401** | Unauthorized |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **export_mock_dataset**
> str export_mock_dataset(type)

DatasetController@exportMock

Export Mock

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
    api_instance = gateway_api_sdk.DatasetsApi(api_client)
    type = 'type_example' # str | type export

    try:
        # DatasetController@exportMock
        api_response = api_instance.export_mock_dataset(type)
        print("The response of DatasetsApi->export_mock_dataset:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetsApi->export_mock_dataset: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **type** | **str**| type export | 

### Return type

**str**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/csv, application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | CSV file |  -  |
**401** | Unauthorized |  -  |
**404** | File Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **export_mock_dataset_v2**
> str export_mock_dataset_v2(type)

DatasetController@exportMock

Export Mock

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
    api_instance = gateway_api_sdk.DatasetsApi(api_client)
    type = 'type_example' # str | 

    try:
        # DatasetController@exportMock
        api_response = api_instance.export_mock_dataset_v2(type)
        print("The response of DatasetsApi->export_mock_dataset_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetsApi->export_mock_dataset_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **type** | **str**|  | 

### Return type

**str**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/csv, application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | CSV file |  -  |
**401** | Unauthorized |  -  |
**404** | File Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_all_datasets**
> FetchAllDatasets200Response fetch_all_datasets(team_id, pid=pid, sort=sort, title=title, status=status)

DatasetController@index

Get All Datasets

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_datasets200_response import FetchAllDatasets200Response
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
    api_instance = gateway_api_sdk.DatasetsApi(api_client)
    team_id = 1 # int | team id
    pid = 'aa588d1c-21e7-42d9-9b60-48e3d6b784a9' # str | get based on a pid (optional)
    sort = 'created:desc' # str | Field and direction (colon separated) to sort by (default: 'created:desc') ... <br/> <br/>         - ?sort=\\<field\\>:\\<direction\\> <br/>         - \\<direction\\> can only be 'asc' or 'desc'  <br/>         - \\<field\\> can only be a valid field for the dataset table that can be ordered on  <br/>         - \\<field\\> can start with the prefix 'metadata.' so that nested values within the field 'metadata'  <br/>             (represented by the GWDM JSON structure) can be used to order on.  <br/>  <br/> (optional)
    title = 'hdr' # str | Three or more characters to filter dataset titles by (optional)
    status = 'ACTIVE' # str | Dataset status to filter by ('ACTIVE', 'DRAFT', 'ARCHIVED') (optional)

    try:
        # DatasetController@index
        api_response = api_instance.fetch_all_datasets(team_id, pid=pid, sort=sort, title=title, status=status)
        print("The response of DatasetsApi->fetch_all_datasets:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetsApi->fetch_all_datasets: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **pid** | **str**| get based on a pid | [optional] 
 **sort** | **str**| Field and direction (colon separated) to sort by (default: &#39;created:desc&#39;) ... &lt;br/&gt; &lt;br/&gt;         - ?sort&#x3D;\\&lt;field\\&gt;:\\&lt;direction\\&gt; &lt;br/&gt;         - \\&lt;direction\\&gt; can only be &#39;asc&#39; or &#39;desc&#39;  &lt;br/&gt;         - \\&lt;field\\&gt; can only be a valid field for the dataset table that can be ordered on  &lt;br/&gt;         - \\&lt;field\\&gt; can start with the prefix &#39;metadata.&#39; so that nested values within the field &#39;metadata&#39;  &lt;br/&gt;             (represented by the GWDM JSON structure) can be used to order on.  &lt;br/&gt;  &lt;br/&gt; | [optional] 
 **title** | **str**| Three or more characters to filter dataset titles by | [optional] 
 **status** | **str**| Dataset status to filter by (&#39;ACTIVE&#39;, &#39;DRAFT&#39;, &#39;ARCHIVED&#39;) | [optional] 

### Return type

[**FetchAllDatasets200Response**](FetchAllDatasets200Response.md)

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

# **fetch_all_datasets_integrations**
> FetchAllDatasets200Response fetch_all_datasets_integrations(team_id, pid=pid, sort=sort, title=title, status=status)

IntegrationDatasetController@index

Get All Datasets

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_datasets200_response import FetchAllDatasets200Response
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
    api_instance = gateway_api_sdk.DatasetsApi(api_client)
    team_id = 1 # int | team id
    pid = 'aa588d1c-21e7-42d9-9b60-48e3d6b784a9' # str | get based on a pid (optional)
    sort = 'created:desc' # str | Field and direction (colon separated) to sort by (default: 'created:desc') ... <br/> <br/>         - ?sort=\\<field\\>:\\<direction\\> <br/>         - \\<direction\\> can only be 'asc' or 'desc'  <br/>         - \\<field\\> can only be a valid field for the dataset table that can be ordered on  <br/>         - \\<field\\> can start with the prefix 'metadata.' so that nested values within the field 'metadata'  <br/>             (represented by the GWDM JSON structure) can be used to order on.  <br/>  <br/> (optional)
    title = 'hdr' # str | Three or more characters to filter dataset titles by (optional)
    status = 'ACTIVE' # str | Dataset status to filter by ('ACTIVE', 'DRAFT', 'ARCHIVED') (optional)

    try:
        # IntegrationDatasetController@index
        api_response = api_instance.fetch_all_datasets_integrations(team_id, pid=pid, sort=sort, title=title, status=status)
        print("The response of DatasetsApi->fetch_all_datasets_integrations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetsApi->fetch_all_datasets_integrations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **pid** | **str**| get based on a pid | [optional] 
 **sort** | **str**| Field and direction (colon separated) to sort by (default: &#39;created:desc&#39;) ... &lt;br/&gt; &lt;br/&gt;         - ?sort&#x3D;\\&lt;field\\&gt;:\\&lt;direction\\&gt; &lt;br/&gt;         - \\&lt;direction\\&gt; can only be &#39;asc&#39; or &#39;desc&#39;  &lt;br/&gt;         - \\&lt;field\\&gt; can only be a valid field for the dataset table that can be ordered on  &lt;br/&gt;         - \\&lt;field\\&gt; can start with the prefix &#39;metadata.&#39; so that nested values within the field &#39;metadata&#39;  &lt;br/&gt;             (represented by the GWDM JSON structure) can be used to order on.  &lt;br/&gt;  &lt;br/&gt; | [optional] 
 **title** | **str**| Three or more characters to filter dataset titles by | [optional] 
 **status** | **str**| Dataset status to filter by (&#39;ACTIVE&#39;, &#39;DRAFT&#39;, &#39;ARCHIVED&#39;) | [optional] 

### Return type

[**FetchAllDatasets200Response**](FetchAllDatasets200Response.md)

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

# **fetch_all_datasets_v2**
> FetchAllDatasets200Response fetch_all_datasets_v2(sort=sort, title=title, status=status, with_metadata=with_metadata)

DatasetController@index

Returns a list of all datasets

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_datasets200_response import FetchAllDatasets200Response
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
    api_instance = gateway_api_sdk.DatasetsApi(api_client)
    sort = 'created:desc' # str | Field and direction (colon separated) to sort by (default: 'created:desc') ... <br/> <br/>         - ?sort=\\<field\\>:\\<direction\\> <br/>         - \\<direction\\> can only be 'asc' or 'desc'  <br/>         - \\<field\\> can only be a valid field for the dataset table that can be ordered on  <br/>         - \\<field\\> can start with the prefix 'metadata.' so that nested values within the field 'metadata'  <br/>             (represented by the GWDM JSON structure) can be used to order on.  <br/>  <br/> (optional)
    title = 'hdr' # str | Three or more characters to filter dataset titles by (optional)
    status = 'ACTIVE' # str | Dataset status to filter by ('ACTIVE', 'DRAFT', 'ARCHIVED') (optional)
    with_metadata = 'true' # str | Boolean whether to return dataset metadata (optional)

    try:
        # DatasetController@index
        api_response = api_instance.fetch_all_datasets_v2(sort=sort, title=title, status=status, with_metadata=with_metadata)
        print("The response of DatasetsApi->fetch_all_datasets_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetsApi->fetch_all_datasets_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sort** | **str**| Field and direction (colon separated) to sort by (default: &#39;created:desc&#39;) ... &lt;br/&gt; &lt;br/&gt;         - ?sort&#x3D;\\&lt;field\\&gt;:\\&lt;direction\\&gt; &lt;br/&gt;         - \\&lt;direction\\&gt; can only be &#39;asc&#39; or &#39;desc&#39;  &lt;br/&gt;         - \\&lt;field\\&gt; can only be a valid field for the dataset table that can be ordered on  &lt;br/&gt;         - \\&lt;field\\&gt; can start with the prefix &#39;metadata.&#39; so that nested values within the field &#39;metadata&#39;  &lt;br/&gt;             (represented by the GWDM JSON structure) can be used to order on.  &lt;br/&gt;  &lt;br/&gt; | [optional] 
 **title** | **str**| Three or more characters to filter dataset titles by | [optional] 
 **status** | **str**| Dataset status to filter by (&#39;ACTIVE&#39;, &#39;DRAFT&#39;, &#39;ARCHIVED&#39;) | [optional] 
 **with_metadata** | **str**| Boolean whether to return dataset metadata | [optional] 

### Return type

[**FetchAllDatasets200Response**](FetchAllDatasets200Response.md)

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

# **fetch_datasets**
> FetchDatasets200Response fetch_datasets(id, export=export, schema_model=schema_model, schema_version=schema_version)

DatasetController@show

Get dataset by id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_datasets200_response import FetchDatasets200Response
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
    api_instance = gateway_api_sdk.DatasetsApi(api_client)
    id = 1 # int | dataset id
    export = 'structuralMetadata' # str | Alternative output schema model. (optional)
    schema_model = 'schema_model_example' # str | Alternative output schema model. (optional)
    schema_version = 'schema_version_example' # str | Alternative output schema version. (optional)

    try:
        # DatasetController@show
        api_response = api_instance.fetch_datasets(id, export=export, schema_model=schema_model, schema_version=schema_version)
        print("The response of DatasetsApi->fetch_datasets:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetsApi->fetch_datasets: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| dataset id | 
 **export** | **str**| Alternative output schema model. | [optional] 
 **schema_model** | **str**| Alternative output schema model. | [optional] 
 **schema_version** | **str**| Alternative output schema version. | [optional] 

### Return type

[**FetchDatasets200Response**](FetchDatasets200Response.md)

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

# **fetch_datasets_integrations**
> FetchDatasets200Response fetch_datasets_integrations(id, schema_model=schema_model, schema_version=schema_version)

IntegrationDatasetController@show

Get dataset by id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_datasets200_response import FetchDatasets200Response
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
    api_instance = gateway_api_sdk.DatasetsApi(api_client)
    id = 1 # int | dataset id
    schema_model = 'schema_model_example' # str | Alternative output schema model. (optional)
    schema_version = 'schema_version_example' # str | Alternative output schema version. (optional)

    try:
        # IntegrationDatasetController@show
        api_response = api_instance.fetch_datasets_integrations(id, schema_model=schema_model, schema_version=schema_version)
        print("The response of DatasetsApi->fetch_datasets_integrations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetsApi->fetch_datasets_integrations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| dataset id | 
 **schema_model** | **str**| Alternative output schema model. | [optional] 
 **schema_version** | **str**| Alternative output schema version. | [optional] 

### Return type

[**FetchDatasets200Response**](FetchDatasets200Response.md)

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

# **fetch_datasets_v2**
> FetchDatasets200Response fetch_datasets_v2(id, export=export, schema_model=schema_model, schema_version=schema_version)

DatasetController@showActive

Get publicly visible dataset by id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_datasets200_response import FetchDatasets200Response
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
    api_instance = gateway_api_sdk.DatasetsApi(api_client)
    id = 1 # int | dataset id
    export = 'structuralMetadata' # str | Set to 'structuralMetadata' to download as CSV. (optional)
    schema_model = 'schema_model_example' # str | Alternative output schema model. (optional)
    schema_version = 'schema_version_example' # str | Alternative output schema version. (optional)

    try:
        # DatasetController@showActive
        api_response = api_instance.fetch_datasets_v2(id, export=export, schema_model=schema_model, schema_version=schema_version)
        print("The response of DatasetsApi->fetch_datasets_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetsApi->fetch_datasets_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| dataset id | 
 **export** | **str**| Set to &#39;structuralMetadata&#39; to download as CSV. | [optional] 
 **schema_model** | **str**| Alternative output schema model. | [optional] 
 **schema_version** | **str**| Alternative output schema version. | [optional] 

### Return type

[**FetchDatasets200Response**](FetchDatasets200Response.md)

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

# **fetch_team_datasets_status**
> FetchAllDatasets200Response fetch_team_datasets_status(team_id, status, sort=sort, with_metadata=with_metadata)

TeamDatasetController@indexStatus

Returns a list of a team's datasets with the given status

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_datasets200_response import FetchAllDatasets200Response
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
    api_instance = gateway_api_sdk.DatasetsApi(api_client)
    team_id = 1 # int | ID of the team to filter by
    status = 'active' # str | Status of the dataset (active, draft, or archived). Defaults to active if not provided. (default to 'active')
    sort = 'created:desc' # str | Field and direction (colon separated) to sort by (default: 'created:desc') ... <br/> <br/>         - ?sort=\\<field\\>:\\<direction\\> <br/>         - \\<direction\\> can only be 'asc' or 'desc'  <br/>         - \\<field\\> can only be a valid field for the dataset table that can be ordered on  <br/>         - \\<field\\> can start with the prefix 'metadata.' so that nested values within the field 'metadata'  <br/>             (represented by the GWDM JSON structure) can be used to order on.  <br/>  <br/> (optional)
    with_metadata = 'true' # str | Boolean whether to return dataset metadata (optional)

    try:
        # TeamDatasetController@indexStatus
        api_response = api_instance.fetch_team_datasets_status(team_id, status, sort=sort, with_metadata=with_metadata)
        print("The response of DatasetsApi->fetch_team_datasets_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetsApi->fetch_team_datasets_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| ID of the team to filter by | 
 **status** | **str**| Status of the dataset (active, draft, or archived). Defaults to active if not provided. | [default to &#39;active&#39;]
 **sort** | **str**| Field and direction (colon separated) to sort by (default: &#39;created:desc&#39;) ... &lt;br/&gt; &lt;br/&gt;         - ?sort&#x3D;\\&lt;field\\&gt;:\\&lt;direction\\&gt; &lt;br/&gt;         - \\&lt;direction\\&gt; can only be &#39;asc&#39; or &#39;desc&#39;  &lt;br/&gt;         - \\&lt;field\\&gt; can only be a valid field for the dataset table that can be ordered on  &lt;br/&gt;         - \\&lt;field\\&gt; can start with the prefix &#39;metadata.&#39; so that nested values within the field &#39;metadata&#39;  &lt;br/&gt;             (represented by the GWDM JSON structure) can be used to order on.  &lt;br/&gt;  &lt;br/&gt; | [optional] 
 **with_metadata** | **str**| Boolean whether to return dataset metadata | [optional] 

### Return type

[**FetchAllDatasets200Response**](FetchAllDatasets200Response.md)

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

# **fetch_team_datasets_v2**
> FetchDatasets200Response fetch_team_datasets_v2(team_id, id, export=export, schema_model=schema_model, schema_version=schema_version)

TeamDatasetController@show

Get dataset by id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_datasets200_response import FetchDatasets200Response
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
    api_instance = gateway_api_sdk.DatasetsApi(api_client)
    team_id = 1 # int | team id
    id = 1 # int | dataset id
    export = 'structuralMetadata' # str | Alternative output schema model. (optional)
    schema_model = 'schema_model_example' # str | Alternative output schema model. (optional)
    schema_version = 'schema_version_example' # str | Alternative output schema version. (optional)

    try:
        # TeamDatasetController@show
        api_response = api_instance.fetch_team_datasets_v2(team_id, id, export=export, schema_model=schema_model, schema_version=schema_version)
        print("The response of DatasetsApi->fetch_team_datasets_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetsApi->fetch_team_datasets_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **id** | **int**| dataset id | 
 **export** | **str**| Alternative output schema model. | [optional] 
 **schema_model** | **str**| Alternative output schema model. | [optional] 
 **schema_version** | **str**| Alternative output schema version. | [optional] 

### Return type

[**FetchDatasets200Response**](FetchDatasets200Response.md)

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

# **patch_datasets**
> DeleteAliases200Response patch_datasets(id, unarchive=unarchive)

DatasetController@edit

Patch dataset by id

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
    api_instance = gateway_api_sdk.DatasetsApi(api_client)
    id = 1 # int | dataset id
    unarchive = 'unarchive_example' # str | Unarchive a dataset (optional)

    try:
        # DatasetController@edit
        api_response = api_instance.patch_datasets(id, unarchive=unarchive)
        print("The response of DatasetsApi->patch_datasets:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetsApi->patch_datasets: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| dataset id | 
 **unarchive** | **str**| Unarchive a dataset | [optional] 

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
**200** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **patch_datasets_integrations**
> DeleteAliases200Response patch_datasets_integrations(id, unarchive=unarchive)

IntegrationDatasetController@edit

Patch dataset by id

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
    api_instance = gateway_api_sdk.DatasetsApi(api_client)
    id = 1 # int | dataset id
    unarchive = 'unarchive_example' # str | Unarchive a dataset (optional)

    try:
        # IntegrationDatasetController@edit
        api_response = api_instance.patch_datasets_integrations(id, unarchive=unarchive)
        print("The response of DatasetsApi->patch_datasets_integrations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetsApi->patch_datasets_integrations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| dataset id | 
 **unarchive** | **str**| Unarchive a dataset | [optional] 

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
**200** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **patch_datasets_v2**
> DeleteAliases200Response patch_datasets_v2(id, patch_datasets_v2_request)

DatasetController@edit

Patch dataset by id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.delete_aliases200_response import DeleteAliases200Response
from gateway_api_sdk.models.patch_datasets_v2_request import PatchDatasetsV2Request
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
    api_instance = gateway_api_sdk.DatasetsApi(api_client)
    id = 1 # int | dataset id
    patch_datasets_v2_request = gateway_api_sdk.PatchDatasetsV2Request() # PatchDatasetsV2Request | 

    try:
        # DatasetController@edit
        api_response = api_instance.patch_datasets_v2(id, patch_datasets_v2_request)
        print("The response of DatasetsApi->patch_datasets_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetsApi->patch_datasets_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| dataset id | 
 **patch_datasets_v2_request** | [**PatchDatasetsV2Request**](PatchDatasetsV2Request.md)|  | 

### Return type

[**DeleteAliases200Response**](DeleteAliases200Response.md)

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

# **patch_team_datasets_v2**
> DeleteAliases200Response patch_team_datasets_v2(team_id, id, patch_datasets_v2_request)

TeamDatasetController@edit

Edit a dataset owned by a team

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.delete_aliases200_response import DeleteAliases200Response
from gateway_api_sdk.models.patch_datasets_v2_request import PatchDatasetsV2Request
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
    api_instance = gateway_api_sdk.DatasetsApi(api_client)
    team_id = 1 # int | team id
    id = 1 # int | dataset id
    patch_datasets_v2_request = gateway_api_sdk.PatchDatasetsV2Request() # PatchDatasetsV2Request | Pass user credentials

    try:
        # TeamDatasetController@edit
        api_response = api_instance.patch_team_datasets_v2(team_id, id, patch_datasets_v2_request)
        print("The response of DatasetsApi->patch_team_datasets_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetsApi->patch_team_datasets_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **id** | **int**| dataset id | 
 **patch_datasets_v2_request** | [**PatchDatasetsV2Request**](PatchDatasetsV2Request.md)| Pass user credentials | 

### Return type

[**DeleteAliases200Response**](DeleteAliases200Response.md)

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

# **update_datasets**
> CreateCategories200Response update_datasets(id, update_datasets_request)

DatasetController@update

Update a dataset with a new dataset version

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_categories200_response import CreateCategories200Response
from gateway_api_sdk.models.update_datasets_request import UpdateDatasetsRequest
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
    api_instance = gateway_api_sdk.DatasetsApi(api_client)
    id = 1 # int | dataset id
    update_datasets_request = gateway_api_sdk.UpdateDatasetsRequest() # UpdateDatasetsRequest | Pass user credentials

    try:
        # DatasetController@update
        api_response = api_instance.update_datasets(id, update_datasets_request)
        print("The response of DatasetsApi->update_datasets:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetsApi->update_datasets: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| dataset id | 
 **update_datasets_request** | [**UpdateDatasetsRequest**](UpdateDatasetsRequest.md)| Pass user credentials | 

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
**201** | Created |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_datasets_integrations**
> FetchDatasets200Response update_datasets_integrations(id, update_datasets_request, input_schema=input_schema, input_version=input_version)

IntegrationDatasetController@update

Update a dataset with a new dataset version

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_datasets200_response import FetchDatasets200Response
from gateway_api_sdk.models.update_datasets_request import UpdateDatasetsRequest
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
    api_instance = gateway_api_sdk.DatasetsApi(api_client)
    id = 1 # int | dataset id
    update_datasets_request = gateway_api_sdk.UpdateDatasetsRequest() # UpdateDatasetsRequest | Pass user credentials
    input_schema = 'HDRUK' # str | Input schema model. (optional)
    input_version = '3.0.0' # str | Input schema version. (optional)

    try:
        # IntegrationDatasetController@update
        api_response = api_instance.update_datasets_integrations(id, update_datasets_request, input_schema=input_schema, input_version=input_version)
        print("The response of DatasetsApi->update_datasets_integrations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetsApi->update_datasets_integrations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| dataset id | 
 **update_datasets_request** | [**UpdateDatasetsRequest**](UpdateDatasetsRequest.md)| Pass user credentials | 
 **input_schema** | **str**| Input schema model. | [optional] 
 **input_version** | **str**| Input schema version. | [optional] 

### Return type

[**FetchDatasets200Response**](FetchDatasets200Response.md)

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

# **update_datasets_v2**
> CreateCategories200Response update_datasets_v2(id, update_datasets_request)

DatasetController@update

Update a dataset with a new dataset version

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_categories200_response import CreateCategories200Response
from gateway_api_sdk.models.update_datasets_request import UpdateDatasetsRequest
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
    api_instance = gateway_api_sdk.DatasetsApi(api_client)
    id = 1 # int | dataset id
    update_datasets_request = gateway_api_sdk.UpdateDatasetsRequest() # UpdateDatasetsRequest | 

    try:
        # DatasetController@update
        api_response = api_instance.update_datasets_v2(id, update_datasets_request)
        print("The response of DatasetsApi->update_datasets_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetsApi->update_datasets_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| dataset id | 
 **update_datasets_request** | [**UpdateDatasetsRequest**](UpdateDatasetsRequest.md)|  | 

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
**201** | Created |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_team_datasets_v2**
> CreateCategories200Response update_team_datasets_v2(team_id, id, patch_datasets_v2_request)

TeamDatasetController@update

Update a team dataset with a new dataset version

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_categories200_response import CreateCategories200Response
from gateway_api_sdk.models.patch_datasets_v2_request import PatchDatasetsV2Request
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
    api_instance = gateway_api_sdk.DatasetsApi(api_client)
    team_id = 1 # int | team id
    id = 1 # int | dataset id
    patch_datasets_v2_request = gateway_api_sdk.PatchDatasetsV2Request() # PatchDatasetsV2Request | Pass user credentials

    try:
        # TeamDatasetController@update
        api_response = api_instance.update_team_datasets_v2(team_id, id, patch_datasets_v2_request)
        print("The response of DatasetsApi->update_team_datasets_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetsApi->update_team_datasets_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **id** | **int**| dataset id | 
 **patch_datasets_v2_request** | [**PatchDatasetsV2Request**](PatchDatasetsV2Request.md)| Pass user credentials | 

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
**201** | Created |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

