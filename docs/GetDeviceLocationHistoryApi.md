# jasperclient.GetDeviceLocationHistoryApi

All URIs are relative to *https://restapi3.jasper.com/rws/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_device_location_history**](GetDeviceLocationHistoryApi.md#get_device_location_history) | **GET** /v{apiVersion}/devices/{iccid}/locationHistory | Get Device Location History during a specified time frame.


# **get_device_location_history**
> get_device_location_history(iccid, api_version, from_date=from_date, to_date=to_date, page_size=page_size, page_number=page_number)

Get Device Location History during a specified time frame.



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
    api_instance = jasperclient.GetDeviceLocationHistoryApi(api_client)
    iccid = 'iccid_example' # str | ICCID of the device
    api_version = '1' # str | Defaults to 1 (default to '1')
    from_date = 'from_date_example' # str | If this is not specified, most recent 2 location records will be returned. </br> The format is yyyy-MM-ddTHH:mm:ssZ </br> Eg: 2018-07-18T17:31:34+00:00 (optional)
    to_date = 'to_date_example' # str | If this is not specified, location history up until the current date will be returned. </br> The format is yyyy-MM-ddTHH:mm:ssZ </br> Eg: 2018-07-18T17:31:34+00:00 (optional)
    page_size = 56 # int | Maximum of 50, defaults to 50 (optional)
    page_number = 56 # int | Defaults to 1 (optional)

    try:
        # Get Device Location History during a specified time frame.
        api_instance.get_device_location_history(iccid, api_version, from_date=from_date, to_date=to_date, page_size=page_size, page_number=page_number)
    except Exception as e:
        print("Exception when calling GetDeviceLocationHistoryApi->get_device_location_history: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **iccid** | **str**| ICCID of the device | 
 **api_version** | **str**| Defaults to 1 | [default to &#39;1&#39;]
 **from_date** | **str**| If this is not specified, most recent 2 location records will be returned. &lt;/br&gt; The format is yyyy-MM-ddTHH:mm:ssZ &lt;/br&gt; Eg: 2018-07-18T17:31:34+00:00 | [optional] 
 **to_date** | **str**| If this is not specified, location history up until the current date will be returned. &lt;/br&gt; The format is yyyy-MM-ddTHH:mm:ssZ &lt;/br&gt; Eg: 2018-07-18T17:31:34+00:00 | [optional] 
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
**401** | Bad credentials |  -  |
**404** | Resource not found |  -  |
**500** | Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

