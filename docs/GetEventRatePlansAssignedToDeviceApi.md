# jasperclient.GetEventRatePlansAssignedToDeviceApi

All URIs are relative to *https://restapi3.jasper.com/rws/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_terminal_events**](GetEventRatePlansAssignedToDeviceApi.md#get_terminal_events) | **GET** /v{apiVersion}/eventplan/{iccid} | List of currently active and future-dated event plans for device.


# **get_terminal_events**
> get_terminal_events(api_version, iccid, page_size=page_size, page_number=page_number)

List of currently active and future-dated event plans for device.



### Example

* Basic Authentication (basicAuth):

```python
import jasperclient
from jasperclient.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://restapi3.jasper.com/rws/api
# See configuration.py for a list of all supported configuration parameters.
configuration = jasperclient.Configuration(
    host = "https://restapi3.jasper.com/rws/api"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = jasperclient.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with jasperclient.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = jasperclient.GetEventRatePlansAssignedToDeviceApi(api_client)
    api_version = '1' # str | Defaults to 1 (default to '1')
    iccid = 'iccid_example' # str | ICCID of the device
    page_size = 56 # int | Maximum of 50, defaults to 50 (optional)
    page_number = 56 # int | Defaults to 1 (optional)

    try:
        # List of currently active and future-dated event plans for device.
        api_instance.get_terminal_events(api_version, iccid, page_size=page_size, page_number=page_number)
    except Exception as e:
        print("Exception when calling GetEventRatePlansAssignedToDeviceApi->get_terminal_events: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_version** | **str**| Defaults to 1 | [default to &#39;1&#39;]
 **iccid** | **str**| ICCID of the device | 
 **page_size** | **int**| Maximum of 50, defaults to 50 | [optional] 
 **page_number** | **int**| Defaults to 1 | [optional] 

### Return type

void (empty response body)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**400** | Invalid request |  -  |
**401** | Invalid credentials |  -  |
**403** | Forbidden |  -  |
**404** | Resource not found |  -  |
**500** | Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

