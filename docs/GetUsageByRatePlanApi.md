# jasperclient.GetUsageByRatePlanApi

All URIs are relative to *https://restapi3.jasper.com/rws/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_usage_by_rate_plan**](GetUsageByRatePlanApi.md#get_usage_by_rate_plan) | **GET** /v{apiVersion}/usages | Get Usage by RatePlan


# **get_usage_by_rate_plan**
> get_usage_by_rate_plan(rate_plan_name, api_version, cycle_start_date=cycle_start_date, usage_type=usage_type, rate_plan_version=rate_plan_version, page_number=page_number, page_size=page_size)

Get Usage by RatePlan



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
    api_instance = jasperclient.GetUsageByRatePlanApi(api_client)
    rate_plan_name = 'rate_plan_name_example' # str | RatePlan Name
    api_version = '1' # str | Defaults to 1 (default to '1')
    cycle_start_date = 'cycle_start_date_example' # str | Filter by start date of a billing cycle.</br> The format is yyyy-MM-ddZ </br> Eg: 2016-11-10Z or 2016-11-10+00:00 (optional)
    usage_type = 'usage_type_example' # str | Data Usage Type. Values can be either one of these - DATA/SMS/VOICE (optional)
    rate_plan_version = 56 # int | RatePlan Version (optional)
    page_number = 1 # int | Defaults to 1 (optional) (default to 1)
    page_size = 50 # int | Defaults to 50 (optional) (default to 50)

    try:
        # Get Usage by RatePlan
        api_instance.get_usage_by_rate_plan(rate_plan_name, api_version, cycle_start_date=cycle_start_date, usage_type=usage_type, rate_plan_version=rate_plan_version, page_number=page_number, page_size=page_size)
    except Exception as e:
        print("Exception when calling GetUsageByRatePlanApi->get_usage_by_rate_plan: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **rate_plan_name** | **str**| RatePlan Name | 
 **api_version** | **str**| Defaults to 1 | [default to &#39;1&#39;]
 **cycle_start_date** | **str**| Filter by start date of a billing cycle.&lt;/br&gt; The format is yyyy-MM-ddZ &lt;/br&gt; Eg: 2016-11-10Z or 2016-11-10+00:00 | [optional] 
 **usage_type** | **str**| Data Usage Type. Values can be either one of these - DATA/SMS/VOICE | [optional] 
 **rate_plan_version** | **int**| RatePlan Version | [optional] 
 **page_number** | **int**| Defaults to 1 | [optional] [default to 1]
 **page_size** | **int**| Defaults to 50 | [optional] [default to 50]

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

