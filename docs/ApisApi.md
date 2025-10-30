# kubernetes.ApisApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_api_versions**](ApisApi.md#get_api_versions) | **GET** /apis/ | 


# **get_api_versions**
> V1APIGroupList get_api_versions()

get available API versions

### Example


```python
import kubernetes
from kubernetes.models.v1_api_group_list import V1APIGroupList
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
    api_instance = kubernetes.ApisApi(api_client)

    try:
        api_response = api_instance.get_api_versions()
        print("The response of ApisApi->get_api_versions:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ApisApi->get_api_versions: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**V1APIGroupList**](V1APIGroupList.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, application/vnd.kubernetes.protobuf, application/yaml

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  -  |
**401** | Unauthorized |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

