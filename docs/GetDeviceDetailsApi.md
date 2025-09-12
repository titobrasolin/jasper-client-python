# jasperclient.GetDeviceDetailsApi

All URIs are relative to *https://restapi3.jasper.com/rws/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_device_by_iccid**](GetDeviceDetailsApi.md#get_device_by_iccid) | **GET** /v{apiVersion}/devices/{iccid} | Return detailed information for a given device.


# **get_device_by_iccid**
> DeviceDetails get_device_by_iccid(iccid, api_version)

Return detailed information for a given device.



### Example

* Basic Authentication (basicAuth):

```python
import jasperclient
from jasperclient.models.device_details import DeviceDetails
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
    api_instance = jasperclient.GetDeviceDetailsApi(api_client)
    iccid = 'iccid_example' # str | ICCID
    api_version = '1' # str | Defaults to 1 (default to '1')

    try:
        # Return detailed information for a given device.
        api_response = api_instance.get_device_by_iccid(iccid, api_version)
        print("The response of GetDeviceDetailsApi->get_device_by_iccid:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GetDeviceDetailsApi->get_device_by_iccid: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **iccid** | **str**| ICCID | 
 **api_version** | **str**| Defaults to 1 | [default to &#39;1&#39;]

### Return type

[**DeviceDetails**](DeviceDetails.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**400** | Invalid request |  -  |
**401** | Bad credentials |  -  |
**404** | Resource not found |  -  |
**500** | Server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

