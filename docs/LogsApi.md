# kubernetes.LogsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**log_file_handler**](LogsApi.md#log_file_handler) | **GET** /logs/{logpath} | 
[**log_file_list_handler**](LogsApi.md#log_file_list_handler) | **GET** /logs/ | 


# **log_file_handler**
> log_file_handler(logpath)

### Example


```python
import kubernetes
from kubernetes.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = kubernetes.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with kubernetes.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = kubernetes.LogsApi(api_client)
    logpath = 'logpath_example' # str | path to the log

    try:
        api_instance.log_file_handler(logpath)
    except Exception as e:
        print("Exception when calling LogsApi->log_file_handler: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **logpath** | **str**| path to the log | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **log_file_list_handler**
> log_file_list_handler()

### Example


```python
import kubernetes
from kubernetes.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = kubernetes.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with kubernetes.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = kubernetes.LogsApi(api_client)

    try:
        api_instance.log_file_list_handler()
    except Exception as e:
        print("Exception when calling LogsApi->log_file_list_handler: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

