# jasperclient.EditEventRatePlansAssignedToDeviceApi

All URIs are relative to *https://restapi3.jasper.com/rws/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**edit_event_instances**](EditEventRatePlansAssignedToDeviceApi.md#edit_event_instances) | **PUT** /v{apiVersion}/editeventplan/{iccid} | Cancel Pending Events for device


# **edit_event_instances**
> edit_event_instances(api_version, iccid, edit_event_instances_request)

Cancel Pending Events for device

### Example

* Basic Authentication (basicAuth):

```python
import jasperclient
from jasperclient.models.edit_event_instances_request import EditEventInstancesRequest
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
    api_instance = jasperclient.EditEventRatePlansAssignedToDeviceApi(api_client)
    api_version = '1' # str |  (default to '1')
    iccid = 'iccid_example' # str | ICCID of the device
    edit_event_instances_request = jasperclient.EditEventInstancesRequest() # EditEventInstancesRequest | Either of the parameters eventID or eventName is required to cancel pending events

    try:
        # Cancel Pending Events for device
        api_instance.edit_event_instances(api_version, iccid, edit_event_instances_request)
    except Exception as e:
        print("Exception when calling EditEventRatePlansAssignedToDeviceApi->edit_event_instances: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_version** | **str**|  | [default to &#39;1&#39;]
 **iccid** | **str**| ICCID of the device | 
 **edit_event_instances_request** | [**EditEventInstancesRequest**](EditEventInstancesRequest.md)| Either of the parameters eventID or eventName is required to cancel pending events | 

### Return type

void (empty response body)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
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

