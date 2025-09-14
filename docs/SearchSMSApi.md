# jasperclient.SearchSMSApi

All URIs are relative to *https://restapi3.jasper.com/rws/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_sms_messages**](SearchSMSApi.md#get_sms_messages) | **GET** /v{apiVersion}/smsMessages | Search for messages that have been sent or received during a specified time frame.


# **get_sms_messages**
> get_sms_messages(from_date, api_version, account_id=account_id, iccid=iccid, to_date=to_date, page_size=page_size, page_number=page_number, msg_type=msg_type)

Search for messages that have been sent or received during a specified time frame.



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
    api_instance = jasperclient.SearchSMSApi(api_client)
    from_date = 'from_date_example' # str | The format is yyyy-MM-ddTHH:mm:ssZ </br> Eg: 2016-04-18T17:31:34+00:00
    api_version = '1' # str | Defaults to 1 (default to '1')
    account_id = 56 # int | Filter by account (optional)
    iccid = 'iccid_example' # str | If specified, search will be limited to this device (optional)
    to_date = 'to_date_example' # str | If this is not specified, messages up until the current date will be returned. </br> The format is yyyy-MM-ddTHH:mm:ssZ </br> Eg: 2016-04-18T17:31:34+00:00 (optional)
    page_size = 50 # int | Maximum of 50, defaults to 50 (optional) (default to 50)
    page_number = 1 # int | Defaults to 1 (optional) (default to 1)
    msg_type = 'msg_type_example' # str | Filter by Msg type (MO/MT) (optional)

    try:
        # Search for messages that have been sent or received during a specified time frame.
        api_instance.get_sms_messages(from_date, api_version, account_id=account_id, iccid=iccid, to_date=to_date, page_size=page_size, page_number=page_number, msg_type=msg_type)
    except Exception as e:
        print("Exception when calling SearchSMSApi->get_sms_messages: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **from_date** | **str**| The format is yyyy-MM-ddTHH:mm:ssZ &lt;/br&gt; Eg: 2016-04-18T17:31:34+00:00 | 
 **api_version** | **str**| Defaults to 1 | [default to &#39;1&#39;]
 **account_id** | **int**| Filter by account | [optional] 
 **iccid** | **str**| If specified, search will be limited to this device | [optional] 
 **to_date** | **str**| If this is not specified, messages up until the current date will be returned. &lt;/br&gt; The format is yyyy-MM-ddTHH:mm:ssZ &lt;/br&gt; Eg: 2016-04-18T17:31:34+00:00 | [optional] 
 **page_size** | **int**| Maximum of 50, defaults to 50 | [optional] [default to 50]
 **page_number** | **int**| Defaults to 1 | [optional] [default to 1]
 **msg_type** | **str**| Filter by Msg type (MO/MT) | [optional] 

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
**500** | Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

