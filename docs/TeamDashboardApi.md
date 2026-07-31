# gateway_api_sdk.TeamDashboardApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**fetch_collections_views_v3**](TeamDashboardApi.md#fetch_collections_views_v3) | **GET** /api/v3/teams/{id}/dashboard/collections/views | TeamDashboardController@collectionViews
[**fetch_dar_applications_application_timeline_v3**](TeamDashboardApi.md#fetch_dar_applications_application_timeline_v3) | **GET** /api/v3/teams/{id}/dar/dashboard/timeline | DataAccessDashboardController@getApplicationTimeline
[**fetch_dar_applications_average_time_to_approval_v3**](TeamDashboardApi.md#fetch_dar_applications_average_time_to_approval_v3) | **GET** /api/v3/teams/{id}/dar/dashboard/average-time | DataAccessDashboardController@getAverageTimeToApproval
[**fetch_dar_applications_current_status_v3**](TeamDashboardApi.md#fetch_dar_applications_current_status_v3) | **GET** /api/v3/teams/{id}/dar/dashboard/status | DataAccessDashboardController@getApplicationStatus
[**fetch_dar_applications_dashboard_export_csv_v3**](TeamDashboardApi.md#fetch_dar_applications_dashboard_export_csv_v3) | **GET** /api/v3/teams/{id}/dar/dashboard/export/csv | DataAccessDashboardController@exportDashboardCsv
[**fetch_dar_applications_dashboard_required_actions_export_csv_v3**](TeamDashboardApi.md#fetch_dar_applications_dashboard_required_actions_export_csv_v3) | **GET** /api/v3/teams/{id}/dar/dashboard/required-actions/export/csv | DataAccessDashboardController@exportRequiredActionsCsv
[**fetch_dar_applications_dashboard_timeline_export_csv_v3**](TeamDashboardApi.md#fetch_dar_applications_dashboard_timeline_export_csv_v3) | **GET** /api/v3/teams/{id}/dar/dashboard/timeline/export/csv | DataAccessDashboardController@exportDashboardTimelineCsv
[**fetch_dar_applications_required_actions_v3**](TeamDashboardApi.md#fetch_dar_applications_required_actions_v3) | **GET** /api/v3/teams/{id}/dar/dashboard/required-actions | DataAccessDashboardController@getRequiredActions
[**fetch_dar_my_applications_v3**](TeamDashboardApi.md#fetch_dar_my_applications_v3) | **GET** /api/v3/teams/{id}/dar/dashboard/count | DataAccessDashboardController@getMyApplications
[**fetch_dashboard_download_csv_v3**](TeamDashboardApi.md#fetch_dashboard_download_csv_v3) | **GET** /api/v3/teams/{id}/dashboard/download/csv | TeamDashboardController@downloadCsv
[**fetch_data_custodians_views_v3**](TeamDashboardApi.md#fetch_data_custodians_views_v3) | **GET** /api/v3/teams/{id}/dashboard/datacustodians/views | TeamDashboardController@datacustodianViews
[**fetch_dataset_views360_v3**](TeamDashboardApi.md#fetch_dataset_views360_v3) | **GET** /api/v3/teams/{id}/dashboard/datasets/views/360 | TeamDashboardController@datasetViews360
[**fetch_dataset_views_top_v3**](TeamDashboardApi.md#fetch_dataset_views_top_v3) | **GET** /api/v3/teams/{id}/dashboard/datasets/views/top | TeamDashboardController@datasetViewsTop
[**fetch_entities_count_v3**](TeamDashboardApi.md#fetch_entities_count_v3) | **GET** /api/v3/teams/{id}/dashboard/{entity}/count | TeamDashboardController@entityCount


# **fetch_collections_views_v3**
> FetchCollectionsViewsV3200Response fetch_collections_views_v3(id, start_date=start_date, end_date=end_date)

TeamDashboardController@collectionViews

Get count of a collection views for a team

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_collections_views_v3200_response import FetchCollectionsViewsV3200Response
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
    api_instance = gateway_api_sdk.TeamDashboardApi(api_client)
    id = 1 # int | Team ID
    start_date = 'Mon Jan 01 00:00:00 UTC 2024' # date | Start date for the reporting interval (Y-m-d). Defaults to one year ago. (optional)
    end_date = 'Tue Dec 31 00:00:00 UTC 2024' # date | End date for the reporting interval (Y-m-d). Defaults to today. (optional)

    try:
        # TeamDashboardController@collectionViews
        api_response = api_instance.fetch_collections_views_v3(id, start_date=start_date, end_date=end_date)
        print("The response of TeamDashboardApi->fetch_collections_views_v3:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamDashboardApi->fetch_collections_views_v3: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Team ID | 
 **start_date** | **date**| Start date for the reporting interval (Y-m-d). Defaults to one year ago. | [optional] 
 **end_date** | **date**| End date for the reporting interval (Y-m-d). Defaults to today. | [optional] 

### Return type

[**FetchCollectionsViewsV3200Response**](FetchCollectionsViewsV3200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_dar_applications_application_timeline_v3**
> CreateWidget201Response fetch_dar_applications_application_timeline_v3(id, start_date=start_date, end_date=end_date)

DataAccessDashboardController@getApplicationTimeline

Get Dar applications timeline for a team

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.create_widget201_response import CreateWidget201Response
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
    api_instance = gateway_api_sdk.TeamDashboardApi(api_client)
    id = 1 # int | Team ID
    start_date = 'Mon Jan 01 00:00:00 UTC 2024' # date | Start date for the reporting interval (Y-m-d). Defaults to one year ago. (optional)
    end_date = 'Tue Dec 31 00:00:00 UTC 2024' # date | End date for the reporting interval (Y-m-d). Defaults to today. (optional)

    try:
        # DataAccessDashboardController@getApplicationTimeline
        api_response = api_instance.fetch_dar_applications_application_timeline_v3(id, start_date=start_date, end_date=end_date)
        print("The response of TeamDashboardApi->fetch_dar_applications_application_timeline_v3:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamDashboardApi->fetch_dar_applications_application_timeline_v3: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Team ID | 
 **start_date** | **date**| Start date for the reporting interval (Y-m-d). Defaults to one year ago. | [optional] 
 **end_date** | **date**| End date for the reporting interval (Y-m-d). Defaults to today. | [optional] 

### Return type

[**CreateWidget201Response**](CreateWidget201Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_dar_applications_average_time_to_approval_v3**
> CreateWidget201Response fetch_dar_applications_average_time_to_approval_v3(id, start_date=start_date, end_date=end_date)

DataAccessDashboardController@getAverageTimeToApproval

Get Dar applications average time to approval for a team

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.create_widget201_response import CreateWidget201Response
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
    api_instance = gateway_api_sdk.TeamDashboardApi(api_client)
    id = 1 # int | Team ID
    start_date = 'Mon Jan 01 00:00:00 UTC 2024' # date | Start date for the reporting interval (Y-m-d). Defaults to one year ago. (optional)
    end_date = 'Tue Dec 31 00:00:00 UTC 2024' # date | End date for the reporting interval (Y-m-d). Defaults to today. (optional)

    try:
        # DataAccessDashboardController@getAverageTimeToApproval
        api_response = api_instance.fetch_dar_applications_average_time_to_approval_v3(id, start_date=start_date, end_date=end_date)
        print("The response of TeamDashboardApi->fetch_dar_applications_average_time_to_approval_v3:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamDashboardApi->fetch_dar_applications_average_time_to_approval_v3: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Team ID | 
 **start_date** | **date**| Start date for the reporting interval (Y-m-d). Defaults to one year ago. | [optional] 
 **end_date** | **date**| End date for the reporting interval (Y-m-d). Defaults to today. | [optional] 

### Return type

[**CreateWidget201Response**](CreateWidget201Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_dar_applications_current_status_v3**
> CreateWidget201Response fetch_dar_applications_current_status_v3(id, start_date=start_date, end_date=end_date)

DataAccessDashboardController@getApplicationStatus

Get Dar applications current status for a team

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.create_widget201_response import CreateWidget201Response
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
    api_instance = gateway_api_sdk.TeamDashboardApi(api_client)
    id = 1 # int | Team ID
    start_date = 'Mon Jan 01 00:00:00 UTC 2024' # date | Start date for the reporting interval (Y-m-d). Defaults to one year ago. (optional)
    end_date = 'Tue Dec 31 00:00:00 UTC 2024' # date | End date for the reporting interval (Y-m-d). Defaults to today. (optional)

    try:
        # DataAccessDashboardController@getApplicationStatus
        api_response = api_instance.fetch_dar_applications_current_status_v3(id, start_date=start_date, end_date=end_date)
        print("The response of TeamDashboardApi->fetch_dar_applications_current_status_v3:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamDashboardApi->fetch_dar_applications_current_status_v3: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Team ID | 
 **start_date** | **date**| Start date for the reporting interval (Y-m-d). Defaults to one year ago. | [optional] 
 **end_date** | **date**| End date for the reporting interval (Y-m-d). Defaults to today. | [optional] 

### Return type

[**CreateWidget201Response**](CreateWidget201Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_dar_applications_dashboard_export_csv_v3**
> CreateWidget201Response fetch_dar_applications_dashboard_export_csv_v3(id, start_date=start_date, end_date=end_date)

DataAccessDashboardController@exportDashboardCsv

Get Dar applications dashboard export csv for a team

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.create_widget201_response import CreateWidget201Response
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
    api_instance = gateway_api_sdk.TeamDashboardApi(api_client)
    id = 1 # int | Team ID
    start_date = 'Mon Jan 01 00:00:00 UTC 2024' # date | Start date for the reporting interval (Y-m-d). Defaults to one year ago. (optional)
    end_date = 'Tue Dec 31 00:00:00 UTC 2024' # date | End date for the reporting interval (Y-m-d). Defaults to today. (optional)

    try:
        # DataAccessDashboardController@exportDashboardCsv
        api_response = api_instance.fetch_dar_applications_dashboard_export_csv_v3(id, start_date=start_date, end_date=end_date)
        print("The response of TeamDashboardApi->fetch_dar_applications_dashboard_export_csv_v3:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamDashboardApi->fetch_dar_applications_dashboard_export_csv_v3: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Team ID | 
 **start_date** | **date**| Start date for the reporting interval (Y-m-d). Defaults to one year ago. | [optional] 
 **end_date** | **date**| End date for the reporting interval (Y-m-d). Defaults to today. | [optional] 

### Return type

[**CreateWidget201Response**](CreateWidget201Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_dar_applications_dashboard_required_actions_export_csv_v3**
> CreateWidget201Response fetch_dar_applications_dashboard_required_actions_export_csv_v3(id)

DataAccessDashboardController@exportRequiredActionsCsv

Get Dar applications dashboard timeline export csv for a team

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.create_widget201_response import CreateWidget201Response
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
    api_instance = gateway_api_sdk.TeamDashboardApi(api_client)
    id = 1 # int | Team ID

    try:
        # DataAccessDashboardController@exportRequiredActionsCsv
        api_response = api_instance.fetch_dar_applications_dashboard_required_actions_export_csv_v3(id)
        print("The response of TeamDashboardApi->fetch_dar_applications_dashboard_required_actions_export_csv_v3:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamDashboardApi->fetch_dar_applications_dashboard_required_actions_export_csv_v3: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Team ID | 

### Return type

[**CreateWidget201Response**](CreateWidget201Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_dar_applications_dashboard_timeline_export_csv_v3**
> CreateWidget201Response fetch_dar_applications_dashboard_timeline_export_csv_v3(id, start_date=start_date, end_date=end_date)

DataAccessDashboardController@exportDashboardTimelineCsv

Get Dar applications dashboard timeline export csv for a team

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.create_widget201_response import CreateWidget201Response
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
    api_instance = gateway_api_sdk.TeamDashboardApi(api_client)
    id = 1 # int | Team ID
    start_date = 'Mon Jan 01 00:00:00 UTC 2024' # date | Start date for the reporting interval (Y-m-d). Defaults to one year ago. (optional)
    end_date = 'Tue Dec 31 00:00:00 UTC 2024' # date | End date for the reporting interval (Y-m-d). Defaults to today. (optional)

    try:
        # DataAccessDashboardController@exportDashboardTimelineCsv
        api_response = api_instance.fetch_dar_applications_dashboard_timeline_export_csv_v3(id, start_date=start_date, end_date=end_date)
        print("The response of TeamDashboardApi->fetch_dar_applications_dashboard_timeline_export_csv_v3:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamDashboardApi->fetch_dar_applications_dashboard_timeline_export_csv_v3: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Team ID | 
 **start_date** | **date**| Start date for the reporting interval (Y-m-d). Defaults to one year ago. | [optional] 
 **end_date** | **date**| End date for the reporting interval (Y-m-d). Defaults to today. | [optional] 

### Return type

[**CreateWidget201Response**](CreateWidget201Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_dar_applications_required_actions_v3**
> CreateWidget201Response fetch_dar_applications_required_actions_v3(id, start_date=start_date, end_date=end_date)

DataAccessDashboardController@getRequiredActions

Get Dar applications required actions for a team

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.create_widget201_response import CreateWidget201Response
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
    api_instance = gateway_api_sdk.TeamDashboardApi(api_client)
    id = 1 # int | Team ID
    start_date = 'Mon Jan 01 00:00:00 UTC 2024' # date | Start date for the reporting interval (Y-m-d). Defaults to one year ago. (optional)
    end_date = 'Tue Dec 31 00:00:00 UTC 2024' # date | End date for the reporting interval (Y-m-d). Defaults to today. (optional)

    try:
        # DataAccessDashboardController@getRequiredActions
        api_response = api_instance.fetch_dar_applications_required_actions_v3(id, start_date=start_date, end_date=end_date)
        print("The response of TeamDashboardApi->fetch_dar_applications_required_actions_v3:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamDashboardApi->fetch_dar_applications_required_actions_v3: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Team ID | 
 **start_date** | **date**| Start date for the reporting interval (Y-m-d). Defaults to one year ago. | [optional] 
 **end_date** | **date**| End date for the reporting interval (Y-m-d). Defaults to today. | [optional] 

### Return type

[**CreateWidget201Response**](CreateWidget201Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_dar_my_applications_v3**
> CreateWidget201Response fetch_dar_my_applications_v3(id, start_date=start_date, end_date=end_date)

DataAccessDashboardController@getMyApplications

Get Dar applications for a team

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.create_widget201_response import CreateWidget201Response
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
    api_instance = gateway_api_sdk.TeamDashboardApi(api_client)
    id = 1 # int | Team ID
    start_date = 'Mon Jan 01 00:00:00 UTC 2024' # date | Start date for the reporting interval (Y-m-d). Defaults to one year ago. (optional)
    end_date = 'Tue Dec 31 00:00:00 UTC 2024' # date | End date for the reporting interval (Y-m-d). Defaults to today. (optional)

    try:
        # DataAccessDashboardController@getMyApplications
        api_response = api_instance.fetch_dar_my_applications_v3(id, start_date=start_date, end_date=end_date)
        print("The response of TeamDashboardApi->fetch_dar_my_applications_v3:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamDashboardApi->fetch_dar_my_applications_v3: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Team ID | 
 **start_date** | **date**| Start date for the reporting interval (Y-m-d). Defaults to one year ago. | [optional] 
 **end_date** | **date**| End date for the reporting interval (Y-m-d). Defaults to today. | [optional] 

### Return type

[**CreateWidget201Response**](CreateWidget201Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_dashboard_download_csv_v3**
> bytes fetch_dashboard_download_csv_v3(id, start_date=start_date, end_date=end_date)

TeamDashboardController@downloadCsv

Download dashboard data custodian in csv format

### Example


```python
import gateway_api_sdk
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
    api_instance = gateway_api_sdk.TeamDashboardApi(api_client)
    id = 1 # int | Team ID
    start_date = 'Mon Jan 01 00:00:00 UTC 2024' # date | Start date for the reporting interval (Y-m-d). Defaults to one year ago. (optional)
    end_date = 'Tue Dec 31 00:00:00 UTC 2024' # date | End date for the reporting interval (Y-m-d). Defaults to today. (optional)

    try:
        # TeamDashboardController@downloadCsv
        api_response = api_instance.fetch_dashboard_download_csv_v3(id, start_date=start_date, end_date=end_date)
        print("The response of TeamDashboardApi->fetch_dashboard_download_csv_v3:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamDashboardApi->fetch_dashboard_download_csv_v3: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Team ID | 
 **start_date** | **date**| Start date for the reporting interval (Y-m-d). Defaults to one year ago. | [optional] 
 **end_date** | **date**| End date for the reporting interval (Y-m-d). Defaults to today. | [optional] 

### Return type

**bytes**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/csv, application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | CSV file download containing dashboard metrics for the team |  -  |
**400** | Invalid team ID |  -  |
**500** | Invalid date interval |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_data_custodians_views_v3**
> FetchCollectionsViewsV3200Response fetch_data_custodians_views_v3(id, start_date=start_date, end_date=end_date)

TeamDashboardController@datacustodianViews

Get count of a data custodian views for a team

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_collections_views_v3200_response import FetchCollectionsViewsV3200Response
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
    api_instance = gateway_api_sdk.TeamDashboardApi(api_client)
    id = 1 # int | Team ID
    start_date = 'Mon Jan 01 00:00:00 UTC 2024' # date | Start date for the reporting interval (Y-m-d). Defaults to one year ago. (optional)
    end_date = 'Tue Dec 31 00:00:00 UTC 2024' # date | End date for the reporting interval (Y-m-d). Defaults to today. (optional)

    try:
        # TeamDashboardController@datacustodianViews
        api_response = api_instance.fetch_data_custodians_views_v3(id, start_date=start_date, end_date=end_date)
        print("The response of TeamDashboardApi->fetch_data_custodians_views_v3:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamDashboardApi->fetch_data_custodians_views_v3: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Team ID | 
 **start_date** | **date**| Start date for the reporting interval (Y-m-d). Defaults to one year ago. | [optional] 
 **end_date** | **date**| End date for the reporting interval (Y-m-d). Defaults to today. | [optional] 

### Return type

[**FetchCollectionsViewsV3200Response**](FetchCollectionsViewsV3200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_dataset_views360_v3**
> FetchDatasetViews360V3200Response fetch_dataset_views360_v3(id, start_date=start_date, end_date=end_date)

TeamDashboardController@datasetViews360

Get count of a datasets views 360 for a team

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_dataset_views360_v3200_response import FetchDatasetViews360V3200Response
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
    api_instance = gateway_api_sdk.TeamDashboardApi(api_client)
    id = 1 # int | Team ID
    start_date = 'Mon Jan 01 00:00:00 UTC 2024' # date | Start date for the reporting interval (Y-m-d). Defaults to one year ago. (optional)
    end_date = 'Tue Dec 31 00:00:00 UTC 2024' # date | End date for the reporting interval (Y-m-d). Defaults to today. (optional)

    try:
        # TeamDashboardController@datasetViews360
        api_response = api_instance.fetch_dataset_views360_v3(id, start_date=start_date, end_date=end_date)
        print("The response of TeamDashboardApi->fetch_dataset_views360_v3:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamDashboardApi->fetch_dataset_views360_v3: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Team ID | 
 **start_date** | **date**| Start date for the reporting interval (Y-m-d). Defaults to one year ago. | [optional] 
 **end_date** | **date**| End date for the reporting interval (Y-m-d). Defaults to today. | [optional] 

### Return type

[**FetchDatasetViews360V3200Response**](FetchDatasetViews360V3200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_dataset_views_top_v3**
> FetchDatasetViewsTopV3200Response fetch_dataset_views_top_v3(id, start_date=start_date, end_date=end_date)

TeamDashboardController@datasetViewsTop

Get count of a datasets views top for a team

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_dataset_views_top_v3200_response import FetchDatasetViewsTopV3200Response
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
    api_instance = gateway_api_sdk.TeamDashboardApi(api_client)
    id = 1 # int | Team ID
    start_date = 'Mon Jan 01 00:00:00 UTC 2024' # date | Start date for the reporting interval (Y-m-d). Defaults to one year ago. (optional)
    end_date = 'Tue Dec 31 00:00:00 UTC 2024' # date | End date for the reporting interval (Y-m-d). Defaults to today. (optional)

    try:
        # TeamDashboardController@datasetViewsTop
        api_response = api_instance.fetch_dataset_views_top_v3(id, start_date=start_date, end_date=end_date)
        print("The response of TeamDashboardApi->fetch_dataset_views_top_v3:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamDashboardApi->fetch_dataset_views_top_v3: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Team ID | 
 **start_date** | **date**| Start date for the reporting interval (Y-m-d). Defaults to one year ago. | [optional] 
 **end_date** | **date**| End date for the reporting interval (Y-m-d). Defaults to today. | [optional] 

### Return type

[**FetchDatasetViewsTopV3200Response**](FetchDatasetViewsTopV3200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_entities_count_v3**
> FetchEntitiesCountV3200Response fetch_entities_count_v3(id, entity, start_date=start_date, end_date=end_date)

TeamDashboardController@entityCount

Get count of a specific entity for a team

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_entities_count_v3200_response import FetchEntitiesCountV3200Response
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
    api_instance = gateway_api_sdk.TeamDashboardApi(api_client)
    id = 1 # int | Team ID
    entity = 'entity_example' # str | Entity type to count
    start_date = 'Mon Jan 01 00:00:00 UTC 2024' # date | Start date for the reporting interval (Y-m-d). Defaults to one year ago. (optional)
    end_date = 'Tue Dec 31 00:00:00 UTC 2024' # date | End date for the reporting interval (Y-m-d). Defaults to today. (optional)

    try:
        # TeamDashboardController@entityCount
        api_response = api_instance.fetch_entities_count_v3(id, entity, start_date=start_date, end_date=end_date)
        print("The response of TeamDashboardApi->fetch_entities_count_v3:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamDashboardApi->fetch_entities_count_v3: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Team ID | 
 **entity** | **str**| Entity type to count | 
 **start_date** | **date**| Start date for the reporting interval (Y-m-d). Defaults to one year ago. | [optional] 
 **end_date** | **date**| End date for the reporting interval (Y-m-d). Defaults to today. | [optional] 

### Return type

[**FetchEntitiesCountV3200Response**](FetchEntitiesCountV3200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

