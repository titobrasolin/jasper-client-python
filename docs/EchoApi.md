# jasperclient.EchoApi

All URIs are relative to *https://restapi3.jasper.com/rws/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_msg**](EchoApi.md#get_msg) | **GET** /v{apiVersion}/echo/{param} | Simply returns a parameter passed by the client.


# **get_msg**
> Hello get_msg(param, api_version)

Simply returns a parameter passed by the client.



### Example

* Basic Authentication (basicAuth):

```python
import jasperclient
from jasperclient.models.hello import Hello
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
    api_instance = jasperclient.EchoApi(api_client)
    param = 'param_example' # str | 
    api_version = '1' # str | Defaults to 1 (default to '1')

    try:
        # Simply returns a parameter passed by the client.
        api_response = api_instance.get_msg(param, api_version)
        print("The response of EchoApi->get_msg:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EchoApi->get_msg: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **param** | **str**|  | 
 **api_version** | **str**| Defaults to 1 | [default to &#39;1&#39;]

### Return type

[**Hello**](Hello.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | successful operation |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

