# jasperclient.GetListOfDeviceSubscriptionDetailsForGivenAccountApi

All URIs are relative to *https://restapi3.jasper.com/rws/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_acct_device_response**](GetListOfDeviceSubscriptionDetailsForGivenAccountApi.md#get_acct_device_response) | **GET** /v{apiVersion}/dynareport/acct/device/subscriptions | Return list of Device Subscription Details for given account.


# **get_acct_device_response**
> get_acct_device_response(api_version, start_date=start_date, end_date=end_date, billing_cycle=billing_cycle, billable=billable, page_number=page_number, page_size=page_size)

Return list of Device Subscription Details for given account.



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
    api_instance = jasperclient.GetListOfDeviceSubscriptionDetailsForGivenAccountApi(api_client)
    api_version = '1' # str | Defaults to 1 (default to '1')
    start_date = 'start_date_example' # str | Start Date. The format is yyyyMMDD. Example: 20240624 (optional)
    end_date = 'end_date_example' # str | End Date. The format is yyyyMMDD. Example: 20240628 (optional)
    billing_cycle = 'billing_cycle_example' # str | Billing Cycle. The format is yyyyMM. Example: 202410 (optional)
    billable = 'billable_example' # str | Billable flag. Valid value can be Y or N. (optional)
    page_number = 1 # int | Page Number (optional) (default to 1)
    page_size = 50 # int | Page Size (optional) (default to 50)

    try:
        # Return list of Device Subscription Details for given account.
        api_instance.get_acct_device_response(api_version, start_date=start_date, end_date=end_date, billing_cycle=billing_cycle, billable=billable, page_number=page_number, page_size=page_size)
    except Exception as e:
        print("Exception when calling GetListOfDeviceSubscriptionDetailsForGivenAccountApi->get_acct_device_response: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_version** | **str**| Defaults to 1 | [default to &#39;1&#39;]
 **start_date** | **str**| Start Date. The format is yyyyMMDD. Example: 20240624 | [optional] 
 **end_date** | **str**| End Date. The format is yyyyMMDD. Example: 20240628 | [optional] 
 **billing_cycle** | **str**| Billing Cycle. The format is yyyyMM. Example: 202410 | [optional] 
 **billable** | **str**| Billable flag. Valid value can be Y or N. | [optional] 
 **page_number** | **int**| Page Number | [optional] [default to 1]
 **page_size** | **int**| Page Size | [optional] [default to 50]

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
**400** | Bad Request |  -  |
**401** | Invalid Credentials |  -  |
**404** | Resource not found |  -  |
**500** | Server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

