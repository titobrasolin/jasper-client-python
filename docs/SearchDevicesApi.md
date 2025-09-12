# jasperclient.SearchDevicesApi

All URIs are relative to *https://restapi3.jasper.com/rws/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**search_devices**](SearchDevicesApi.md#search_devices) | **GET** /v{apiVersion}/devices | Search for devices based on various filters.


# **search_devices**
> search_devices(api_version, modified_since, account_id=account_id, modified_till=modified_till, status=status, account_custom1=account_custom1, account_custom2=account_custom2, account_custom3=account_custom3, account_custom4=account_custom4, account_custom5=account_custom5, account_custom6=account_custom6, account_custom7=account_custom7, account_custom8=account_custom8, account_custom9=account_custom9, account_custom10=account_custom10, operator_custom1=operator_custom1, operator_custom2=operator_custom2, operator_custom3=operator_custom3, operator_custom4=operator_custom4, operator_custom5=operator_custom5, customer_custom1=customer_custom1, customer_custom2=customer_custom2, customer_custom3=customer_custom3, customer_custom4=customer_custom4, customer_custom5=customer_custom5, page_size=page_size, page_number=page_number)

Search for devices based on various filters.



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
    api_instance = jasperclient.SearchDevicesApi(api_client)
    api_version = '1' # str | Defaults to 1 (default to '1')
    modified_since = 'modified_since_example' # str | Filter by time since last modification was made to device.</br> The format is yyyy-MM-ddTHH:mm:ssZ </br> Eg: 2016-04-18T17:31:34+00:00
    account_id = 56 # int | Filter by account (optional)
    modified_till = 'modified_till_example' # str | Filter by time till last modification was made to device.</br> The format is yyyy-MM-ddTHH:mm:ssZ </br> Eg: 2016-05-18T17:31:34+00:00 (optional)
    status = 'status_example' # str | Filter by device status (optional)
    account_custom1 = 'account_custom1_example' # str | Filter by account custom field 1 (optional)
    account_custom2 = 'account_custom2_example' # str | Filter by account custom field 2 (optional)
    account_custom3 = 'account_custom3_example' # str | Filter by account custom field 3 (optional)
    account_custom4 = 'account_custom4_example' # str | Filter by account custom field 4 (optional)
    account_custom5 = 'account_custom5_example' # str | Filter by account custom field 5 (optional)
    account_custom6 = 'account_custom6_example' # str | Filter by account custom field 6 (optional)
    account_custom7 = 'account_custom7_example' # str | Filter by account custom field 7 (optional)
    account_custom8 = 'account_custom8_example' # str | Filter by account custom field 8 (optional)
    account_custom9 = 'account_custom9_example' # str | Filter by account custom field 9 (optional)
    account_custom10 = 'account_custom10_example' # str | Filter by account custom field 10 (optional)
    operator_custom1 = 'operator_custom1_example' # str | Filter by operator custom field 1 (optional)
    operator_custom2 = 'operator_custom2_example' # str | Filter by operator custom field 2 (optional)
    operator_custom3 = 'operator_custom3_example' # str | Filter by operator custom field 3 (optional)
    operator_custom4 = 'operator_custom4_example' # str | Filter by operator custom field 4 (optional)
    operator_custom5 = 'operator_custom5_example' # str | Filter by operator custom field 5 (optional)
    customer_custom1 = 'customer_custom1_example' # str | Filter by customer custom field 1 (optional)
    customer_custom2 = 'customer_custom2_example' # str | Filter by customer custom field 2 (optional)
    customer_custom3 = 'customer_custom3_example' # str | Filter by customer custom field 3 (optional)
    customer_custom4 = 'customer_custom4_example' # str | Filter by customer custom field 4 (optional)
    customer_custom5 = 'customer_custom5_example' # str | Filter by customer custom field 5 (optional)
    page_size = 50 # int | Maximum of 50, defaults to 50 (optional) (default to 50)
    page_number = 1 # int | Defaults to 1 (optional) (default to 1)

    try:
        # Search for devices based on various filters.
        api_instance.search_devices(api_version, modified_since, account_id=account_id, modified_till=modified_till, status=status, account_custom1=account_custom1, account_custom2=account_custom2, account_custom3=account_custom3, account_custom4=account_custom4, account_custom5=account_custom5, account_custom6=account_custom6, account_custom7=account_custom7, account_custom8=account_custom8, account_custom9=account_custom9, account_custom10=account_custom10, operator_custom1=operator_custom1, operator_custom2=operator_custom2, operator_custom3=operator_custom3, operator_custom4=operator_custom4, operator_custom5=operator_custom5, customer_custom1=customer_custom1, customer_custom2=customer_custom2, customer_custom3=customer_custom3, customer_custom4=customer_custom4, customer_custom5=customer_custom5, page_size=page_size, page_number=page_number)
    except Exception as e:
        print("Exception when calling SearchDevicesApi->search_devices: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_version** | **str**| Defaults to 1 | [default to &#39;1&#39;]
 **modified_since** | **str**| Filter by time since last modification was made to device.&lt;/br&gt; The format is yyyy-MM-ddTHH:mm:ssZ &lt;/br&gt; Eg: 2016-04-18T17:31:34+00:00 | 
 **account_id** | **int**| Filter by account | [optional] 
 **modified_till** | **str**| Filter by time till last modification was made to device.&lt;/br&gt; The format is yyyy-MM-ddTHH:mm:ssZ &lt;/br&gt; Eg: 2016-05-18T17:31:34+00:00 | [optional] 
 **status** | **str**| Filter by device status | [optional] 
 **account_custom1** | **str**| Filter by account custom field 1 | [optional] 
 **account_custom2** | **str**| Filter by account custom field 2 | [optional] 
 **account_custom3** | **str**| Filter by account custom field 3 | [optional] 
 **account_custom4** | **str**| Filter by account custom field 4 | [optional] 
 **account_custom5** | **str**| Filter by account custom field 5 | [optional] 
 **account_custom6** | **str**| Filter by account custom field 6 | [optional] 
 **account_custom7** | **str**| Filter by account custom field 7 | [optional] 
 **account_custom8** | **str**| Filter by account custom field 8 | [optional] 
 **account_custom9** | **str**| Filter by account custom field 9 | [optional] 
 **account_custom10** | **str**| Filter by account custom field 10 | [optional] 
 **operator_custom1** | **str**| Filter by operator custom field 1 | [optional] 
 **operator_custom2** | **str**| Filter by operator custom field 2 | [optional] 
 **operator_custom3** | **str**| Filter by operator custom field 3 | [optional] 
 **operator_custom4** | **str**| Filter by operator custom field 4 | [optional] 
 **operator_custom5** | **str**| Filter by operator custom field 5 | [optional] 
 **customer_custom1** | **str**| Filter by customer custom field 1 | [optional] 
 **customer_custom2** | **str**| Filter by customer custom field 2 | [optional] 
 **customer_custom3** | **str**| Filter by customer custom field 3 | [optional] 
 **customer_custom4** | **str**| Filter by customer custom field 4 | [optional] 
 **customer_custom5** | **str**| Filter by customer custom field 5 | [optional] 
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
**500** | Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

