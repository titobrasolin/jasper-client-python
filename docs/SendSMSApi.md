# jasperclient.SendSMSApi

All URIs are relative to *https://restapi3.jasper.com/rws/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**send_sms_messages**](SendSMSApi.md#send_sms_messages) | **POST** /v{apiVersion}/devices/{iccid}/smsMessages | Send SMS message to a device.


# **send_sms_messages**
> send_sms_messages(iccid, api_version, send_sms_messages_request=send_sms_messages_request)

Send SMS message to a device.



### Example

* Basic Authentication (basicAuth):

```python
import jasperclient
from jasperclient.models.send_sms_messages_request import SendSmsMessagesRequest
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
    api_instance = jasperclient.SendSMSApi(api_client)
    iccid = 'iccid_example' # str | ICCID
    api_version = '1' # str | Defaults to 1 (default to '1')
    send_sms_messages_request = jasperclient.SendSmsMessagesRequest() # SendSmsMessagesRequest |  (optional)

    try:
        # Send SMS message to a device.
        api_instance.send_sms_messages(iccid, api_version, send_sms_messages_request=send_sms_messages_request)
    except Exception as e:
        print("Exception when calling SendSMSApi->send_sms_messages: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **iccid** | **str**| ICCID | 
 **api_version** | **str**| Defaults to 1 | [default to &#39;1&#39;]
 **send_sms_messages_request** | [**SendSmsMessagesRequest**](SendSmsMessagesRequest.md)|  | [optional] 

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
**401** | Bad credentials |  -  |
**404** | Resource not found |  -  |
**500** | Server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

