# jasperclient.GetDeviceAuditTrailsApi

All URIs are relative to *https://restapi3.jasper.com/rws/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_device_audit_trails**](GetDeviceAuditTrailsApi.md#get_device_audit_trails) | **GET** /v{apiVersion}/devices/{iccid}/auditTrails | Retrieve audit history for a device based on various filters.


# **get_device_audit_trails**
> get_device_audit_trails(iccid, api_version, days_of_history=days_of_history, page_size=page_size, page_number=page_number)

Retrieve audit history for a device based on various filters.



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
    api_instance = jasperclient.GetDeviceAuditTrailsApi(api_client)
    iccid = 'iccid_example' # str | ICCID
    api_version = '1' # str | Defaults to 1 (default to '1')
    days_of_history = 30 # int | Maximum allowed 365, Defaults to 30 (optional) (default to 30)
    page_size = 50 # int | Maximum of 50, defaults to 50 (optional) (default to 50)
    page_number = 1 # int | Defaults to 1 (optional) (default to 1)

    try:
        # Retrieve audit history for a device based on various filters.
        api_instance.get_device_audit_trails(iccid, api_version, days_of_history=days_of_history, page_size=page_size, page_number=page_number)
    except Exception as e:
        print("Exception when calling GetDeviceAuditTrailsApi->get_device_audit_trails: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **iccid** | **str**| ICCID | 
 **api_version** | **str**| Defaults to 1 | [default to &#39;1&#39;]
 **days_of_history** | **int**| Maximum allowed 365, Defaults to 30 | [optional] [default to 30]
 **page_size** | **int**| Maximum of 50, defaults to 50 | [optional] [default to 50]
 **page_number** | **int**| Defaults to 1 | [optional] [default to 1]

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
**401** | Bad credentials |  -  |
**404** | Resource not found |  -  |
**500** | Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

