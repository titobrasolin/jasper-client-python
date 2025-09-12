# jasperclient.GetListOfTOPKUsageDetailsGroupByCarrierCountryRatePlanRatingZoneForGivenAccountApi

All URIs are relative to *https://restapi3.jasper.com/rws/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_top_k_usage_by_account**](GetListOfTOPKUsageDetailsGroupByCarrierCountryRatePlanRatingZoneForGivenAccountApi.md#get_top_k_usage_by_account) | **GET** /v{apiVersion}/dynareport/acct/topk/usage | Return list of TOP K Usage Details Group by Carrier, Country, RatePlan, RatingZone for given account.


# **get_top_k_usage_by_account**
> get_top_k_usage_by_account(metrics, api_version, k=k, start_date=start_date, end_date=end_date, billing_cycle=billing_cycle, group_by=group_by, sorted_by=sorted_by, sort_direction=sort_direction, page_number=page_number, page_size=page_size)

Return list of TOP K Usage Details Group by Carrier, Country, RatePlan, RatingZone for given account.



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
    api_instance = jasperclient.GetListOfTOPKUsageDetailsGroupByCarrierCountryRatePlanRatingZoneForGivenAccountApi(api_client)
    metrics = ['metrics_example'] # List[str] | Metrics. Example: data,sms,voice,smt,smo,vmo,vmt. Accepts list of string.
    api_version = '1' # str | Defaults to 1 (default to '1')
    k = 3.4 # float | top K, Default value is 10. Max limit is 100 (optional)
    start_date = 'start_date_example' # str | Start Date. The format is yyyyMMDD. Example: 20240624 (optional)
    end_date = 'end_date_example' # str | End Date. The format is yyyyMMDD. Example: 20240628 (optional)
    billing_cycle = 'billing_cycle_example' # str | Billing Cycle. The format is yyyyMM. Example: 202410 (optional)
    group_by = ['group_by_example'] # List[str] | Group By carrier,country,RatePlan,RatingZone. Example: carrier,country,ratePlan,ratingZone. Accepts list of string. (optional)
    sorted_by = 'account' # str | Sorted By. Example: account, data, sms, voice, smt, smo, vmt, vmo (optional) (default to 'account')
    sort_direction = 'desc' # str | Sort Direction (optional) (default to 'desc')
    page_number = 56 # int | Page Number (optional)
    page_size = 56 # int | Page Size (optional)

    try:
        # Return list of TOP K Usage Details Group by Carrier, Country, RatePlan, RatingZone for given account.
        api_instance.get_top_k_usage_by_account(metrics, api_version, k=k, start_date=start_date, end_date=end_date, billing_cycle=billing_cycle, group_by=group_by, sorted_by=sorted_by, sort_direction=sort_direction, page_number=page_number, page_size=page_size)
    except Exception as e:
        print("Exception when calling GetListOfTOPKUsageDetailsGroupByCarrierCountryRatePlanRatingZoneForGivenAccountApi->get_top_k_usage_by_account: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **metrics** | [**List[str]**](str.md)| Metrics. Example: data,sms,voice,smt,smo,vmo,vmt. Accepts list of string. | 
 **api_version** | **str**| Defaults to 1 | [default to &#39;1&#39;]
 **k** | **float**| top K, Default value is 10. Max limit is 100 | [optional] 
 **start_date** | **str**| Start Date. The format is yyyyMMDD. Example: 20240624 | [optional] 
 **end_date** | **str**| End Date. The format is yyyyMMDD. Example: 20240628 | [optional] 
 **billing_cycle** | **str**| Billing Cycle. The format is yyyyMM. Example: 202410 | [optional] 
 **group_by** | [**List[str]**](str.md)| Group By carrier,country,RatePlan,RatingZone. Example: carrier,country,ratePlan,ratingZone. Accepts list of string. | [optional] 
 **sorted_by** | **str**| Sorted By. Example: account, data, sms, voice, smt, smo, vmt, vmo | [optional] [default to &#39;account&#39;]
 **sort_direction** | **str**| Sort Direction | [optional] [default to &#39;desc&#39;]
 **page_number** | **int**| Page Number | [optional] 
 **page_size** | **int**| Page Size | [optional] 

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

