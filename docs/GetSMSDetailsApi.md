# jasperclient.GetSMSDetailsApi

All URIs are relative to *https://restapi3.jasper.com/rws/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_sms_message_detail**](GetSMSDetailsApi.md#get_sms_message_detail) | **GET** /v{apiVersion}/smsMessages/{smsMsgId} | Returns detailed information about a message.


# **get_sms_message_detail**
> get_sms_message_detail(sms_msg_id, api_version, message_encoding=message_encoding)

Returns detailed information about a message.



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
    api_instance = jasperclient.GetSMSDetailsApi(api_client)
    sms_msg_id = 'sms_msg_id_example' # str | SMS Message ID
    api_version = '1' # str | Defaults to 1 (default to '1')
    message_encoding = 'message_encoding_example' # str | LITERAL(default) or BASE64 (optional)

    try:
        # Returns detailed information about a message.
        api_instance.get_sms_message_detail(sms_msg_id, api_version, message_encoding=message_encoding)
    except Exception as e:
        print("Exception when calling GetSMSDetailsApi->get_sms_message_detail: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sms_msg_id** | **str**| SMS Message ID | 
 **api_version** | **str**| Defaults to 1 | [default to &#39;1&#39;]
 **message_encoding** | **str**| LITERAL(default) or BASE64 | [optional] 

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
**500** | Server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

