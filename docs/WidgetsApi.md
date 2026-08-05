# gateway_api_sdk.WidgetsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_widget**](WidgetsApi.md#create_widget) | **POST** /api/v1/teams/{teamId}/widgets | Create a new widget
[**delete_widget**](WidgetsApi.md#delete_widget) | **DELETE** /api/v1/teams/{teamId}/widgets/{id} | Delete a widget
[**fetch_all_widgets**](WidgetsApi.md#fetch_all_widgets) | **GET** /api/v1/teams/{teamId}/widgets | WidgetController@index
[**fetch_widget**](WidgetsApi.md#fetch_widget) | **GET** /api/v1/teams/{teamId}/widgets/{id} | WidgetController@retrieve
[**fetch_widget_data_sources**](WidgetsApi.md#fetch_widget_data_sources) | **GET** /api/v1/teams/{teamId}/widgets/data | WidgetController@getWidgetData
[**retrieve_widget_data**](WidgetsApi.md#retrieve_widget_data) | **GET** /api/v1/teams/{teamId}/widgets/{id}/data | Retrieve data related to a widget
[**track_widget_event**](WidgetsApi.md#track_widget_event) | **POST** /api/v1/teams/{teamId}/widgets/{id}/track | Record a widget analytics event
[**update_widget**](WidgetsApi.md#update_widget) | **PATCH** /api/v1/teams/{teamId}/widgets/{id} | Update an existing widget
[**widget_analytics**](WidgetsApi.md#widget_analytics) | **GET** /api/v1/teams/{teamId}/widgets/analytics | Get widget analytics for a team


# **create_widget**
> CreateWidget201Response create_widget(team_id, create_widget_request)

Create a new widget

Creates a new widget for a given team

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_widget201_response import CreateWidget201Response
from gateway_api_sdk.models.create_widget_request import CreateWidgetRequest
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
    api_instance = gateway_api_sdk.WidgetsApi(api_client)
    team_id = 5 # int | Team ID the widget belongs to
    create_widget_request = gateway_api_sdk.CreateWidgetRequest() # CreateWidgetRequest | 

    try:
        # Create a new widget
        api_response = api_instance.create_widget(team_id, create_widget_request)
        print("The response of WidgetsApi->create_widget:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WidgetsApi->create_widget: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team ID the widget belongs to | 
 **create_widget_request** | [**CreateWidgetRequest**](CreateWidgetRequest.md)|  | 

### Return type

[**CreateWidget201Response**](CreateWidget201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Widget created successfully |  -  |
**400** | Validation failed |  -  |
**500** | Server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_widget**
> DeleteApplications200Response delete_widget(team_id, id)

Delete a widget

Soft delete a widget belonging to a specific team

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
    api_instance = gateway_api_sdk.WidgetsApi(api_client)
    team_id = 5 # int | Team ID
    id = 1 # int | Widget ID

    try:
        # Delete a widget
        api_response = api_instance.delete_widget(team_id, id)
        print("The response of WidgetsApi->delete_widget:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WidgetsApi->delete_widget: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team ID | 
 **id** | **int**| Widget ID | 

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
**404** | Widget not found |  -  |
**200** | Widget deleted successfully |  -  |
**500** | Server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_all_widgets**
> FetchAllWidgets200Response fetch_all_widgets(team_id)

WidgetController@index

Get All Widgets

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_widgets200_response import FetchAllWidgets200Response
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
    api_instance = gateway_api_sdk.WidgetsApi(api_client)
    team_id = 56 # int | Team ID

    try:
        # WidgetController@index
        api_response = api_instance.fetch_all_widgets(team_id)
        print("The response of WidgetsApi->fetch_all_widgets:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WidgetsApi->fetch_all_widgets: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team ID | 

### Return type

[**FetchAllWidgets200Response**](FetchAllWidgets200Response.md)

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

# **fetch_widget**
> FetchWidget200Response fetch_widget(team_id, id)

WidgetController@retrieve

Get a single Widget

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_widget200_response import FetchWidget200Response
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
    api_instance = gateway_api_sdk.WidgetsApi(api_client)
    team_id = 56 # int | Team ID
    id = 56 # int | Widget ID

    try:
        # WidgetController@retrieve
        api_response = api_instance.fetch_widget(team_id, id)
        print("The response of WidgetsApi->fetch_widget:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WidgetsApi->fetch_widget: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team ID | 
 **id** | **int**| Widget ID | 

### Return type

[**FetchWidget200Response**](FetchWidget200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |
**404** | Widget not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_widget_data_sources**
> FetchWidgetDataSources200Response fetch_widget_data_sources(team_id, team_ids)

WidgetController@getWidgetData

Fetch lightweight data (id, name, etc.) for multiple teams across datasets, tools, collections, and DURS

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_widget_data_sources200_response import FetchWidgetDataSources200Response
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
    api_instance = gateway_api_sdk.WidgetsApi(api_client)
    team_id = 56 # int | Team ID
    team_ids = '1,2,3' # str | Comma-separated list of team IDs to filter data

    try:
        # WidgetController@getWidgetData
        api_response = api_instance.fetch_widget_data_sources(team_id, team_ids)
        print("The response of WidgetsApi->fetch_widget_data_sources:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WidgetsApi->fetch_widget_data_sources: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team ID | 
 **team_ids** | **str**| Comma-separated list of team IDs to filter data | 

### Return type

[**FetchWidgetDataSources200Response**](FetchWidgetDataSources200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Aggregated data retrieved successfully |  -  |
**400** | Invalid or missing teamIds parameter |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **retrieve_widget_data**
> RetrieveWidgetData200Response retrieve_widget_data(team_id, id, domain_origin)

Retrieve data related to a widget

Fetches datasets, data uses, scripts, and collections linked to a widget

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.retrieve_widget_data200_response import RetrieveWidgetData200Response
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
    api_instance = gateway_api_sdk.WidgetsApi(api_client)
    team_id = 56 # int | Team ID
    id = 56 # int | Widget ID
    domain_origin = 'https://example.com' # str | Optional domain URL to check against the widget's permitted_domains list

    try:
        # Retrieve data related to a widget
        api_response = api_instance.retrieve_widget_data(team_id, id, domain_origin)
        print("The response of WidgetsApi->retrieve_widget_data:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WidgetsApi->retrieve_widget_data: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team ID | 
 **id** | **int**| Widget ID | 
 **domain_origin** | **str**| Optional domain URL to check against the widget&#39;s permitted_domains list | 

### Return type

[**RetrieveWidgetData200Response**](RetrieveWidgetData200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**403** | Forbidden — domain not permitted for this widget |  -  |
**200** | Widget data retrieved successfully |  -  |
**404** | Widget not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **track_widget_event**
> track_widget_event(team_id, id, track_widget_event_request)

Record a widget analytics event

Public endpoint for frontend clients to record user interactions with a widget (page views, code copies, gateway clicks, searches). No authentication required.

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.track_widget_event_request import TrackWidgetEventRequest
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
    api_instance = gateway_api_sdk.WidgetsApi(api_client)
    team_id = 56 # int | 
    id = 56 # int | 
    track_widget_event_request = gateway_api_sdk.TrackWidgetEventRequest() # TrackWidgetEventRequest | 

    try:
        # Record a widget analytics event
        api_instance.track_widget_event(team_id, id, track_widget_event_request)
    except Exception as e:
        print("Exception when calling WidgetsApi->track_widget_event: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**|  | 
 **id** | **int**|  | 
 **track_widget_event_request** | [**TrackWidgetEventRequest**](TrackWidgetEventRequest.md)|  | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**204** | Event recorded |  -  |
**404** | Widget not found |  -  |
**422** | Validation error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_widget**
> UpdateWidget200Response update_widget(team_id, id, update_widget_request=update_widget_request)

Update an existing widget

Updates an existing widget for a given team ID

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.update_widget200_response import UpdateWidget200Response
from gateway_api_sdk.models.update_widget_request import UpdateWidgetRequest
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
    api_instance = gateway_api_sdk.WidgetsApi(api_client)
    team_id = 1 # int | Team ID
    id = 12 # int | Widget ID
    update_widget_request = gateway_api_sdk.UpdateWidgetRequest() # UpdateWidgetRequest |  (optional)

    try:
        # Update an existing widget
        api_response = api_instance.update_widget(team_id, id, update_widget_request=update_widget_request)
        print("The response of WidgetsApi->update_widget:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WidgetsApi->update_widget: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team ID | 
 **id** | **int**| Widget ID | 
 **update_widget_request** | [**UpdateWidgetRequest**](UpdateWidgetRequest.md)|  | [optional] 

### Return type

[**UpdateWidget200Response**](UpdateWidget200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Widget successfully updated |  -  |
**404** | Widget not found |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **widget_analytics**
> WidgetAnalytics200Response widget_analytics(team_id, var_from=var_from, to=to, group_by=group_by)

Get widget analytics for a team

Returns aggregated event counts per widget, per event type, and over time. Supports date range filtering and time-based grouping.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.widget_analytics200_response import WidgetAnalytics200Response
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
    api_instance = gateway_api_sdk.WidgetsApi(api_client)
    team_id = 56 # int | 
    var_from = '2026-01-01' # str | Start date (Y-m-d) (optional)
    to = '2026-06-30' # str | End date (Y-m-d) (optional)
    group_by = 'day' # str | Time granularity (optional) (default to 'day')

    try:
        # Get widget analytics for a team
        api_response = api_instance.widget_analytics(team_id, var_from=var_from, to=to, group_by=group_by)
        print("The response of WidgetsApi->widget_analytics:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WidgetsApi->widget_analytics: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**|  | 
 **var_from** | **str**| Start date (Y-m-d) | [optional] 
 **to** | **str**| End date (Y-m-d) | [optional] 
 **group_by** | **str**| Time granularity | [optional] [default to &#39;day&#39;]

### Return type

[**WidgetAnalytics200Response**](WidgetAnalytics200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Analytics data |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

