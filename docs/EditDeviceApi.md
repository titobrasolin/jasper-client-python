# jasperclient.EditDeviceApi

All URIs are relative to *https://restapi3.jasper.com/rws/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**edit_device**](EditDeviceApi.md#edit_device) | **PUT** /v{apiVersion}/devices/{iccid} | Modify any device attributes such as Status, Rate Plan, Communication Plan, Custom Fields and other identifiers.


# **edit_device**
> edit_device(iccid, api_version, device_edit_model)

Modify any device attributes such as Status, Rate Plan, Communication Plan, Custom Fields and other identifiers.



### Example

* Basic Authentication (basicAuth):

```python
import jasperclient
from jasperclient.models.device_edit_model import DeviceEditModel
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
    api_instance = jasperclient.EditDeviceApi(api_client)
    iccid = 'iccid_example' # str | ICCID
    api_version = '1' # str | Defaults to 1 (default to '1')
    device_edit_model = jasperclient.DeviceEditModel() # DeviceEditModel | At least one parameter is required

    try:
        # Modify any device attributes such as Status, Rate Plan, Communication Plan, Custom Fields and other identifiers.
        api_instance.edit_device(iccid, api_version, device_edit_model)
    except Exception as e:
        print("Exception when calling EditDeviceApi->edit_device: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **iccid** | **str**| ICCID | 
 **api_version** | **str**| Defaults to 1 | [default to &#39;1&#39;]
 **device_edit_model** | [**DeviceEditModel**](DeviceEditModel.md)| At least one parameter is required | 

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
**202** | Accepted |  -  |
**400** | Invalid request |  -  |
**401** | Invalid credentials |  -  |
**404** | Resource not found |  -  |
**500** | Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

