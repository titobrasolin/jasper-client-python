# jasperclient.CustomersApi

All URIs are relative to *https://restapi3.jasper.com/rws/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_customer**](CustomersApi.md#create_customer) | **POST** /v{apiVersion}/customers | Creates a customer
[**get_customer_details**](CustomersApi.md#get_customer_details) | **GET** /v{apiVersion}/customers/{customerId} | Get details for a given customerId
[**update_customer**](CustomersApi.md#update_customer) | **PUT** /v{apiVersion}/customers/{customerId} | Edits a customer


# **create_customer**
> create_customer(api_version, customer_dto)

Creates a customer

Creates a customer

### Example

* Basic Authentication (basicAuth):

```python
import jasperclient
from jasperclient.models.customer_dto import CustomerDTO
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
    api_instance = jasperclient.CustomersApi(api_client)
    api_version = '1' # str | Defaults to 1 (default to '1')
    customer_dto = jasperclient.CustomerDTO() # CustomerDTO | Customer Details

    try:
        # Creates a customer
        api_instance.create_customer(api_version, customer_dto)
    except Exception as e:
        print("Exception when calling CustomersApi->create_customer: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_version** | **str**| Defaults to 1 | [default to &#39;1&#39;]
 **customer_dto** | [**CustomerDTO**](CustomerDTO.md)| Customer Details | 

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

# **get_customer_details**
> get_customer_details(customer_id, api_version)

Get details for a given customerId

Get details for a given customerId

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
    api_instance = jasperclient.CustomersApi(api_client)
    customer_id = 'customer_id_example' # str | Customer Id
    api_version = '1' # str | Defaults to 1 (default to '1')

    try:
        # Get details for a given customerId
        api_instance.get_customer_details(customer_id, api_version)
    except Exception as e:
        print("Exception when calling CustomersApi->get_customer_details: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customer_id** | **str**| Customer Id | 
 **api_version** | **str**| Defaults to 1 | [default to &#39;1&#39;]

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

# **update_customer**
> update_customer(customer_id, api_version, customer_dto)

Edits a customer

Edits a customer

### Example

* Basic Authentication (basicAuth):

```python
import jasperclient
from jasperclient.models.customer_dto import CustomerDTO
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
    api_instance = jasperclient.CustomersApi(api_client)
    customer_id = 'customer_id_example' # str | Customer Id
    api_version = '1' # str | Defaults to 1 (default to '1')
    customer_dto = jasperclient.CustomerDTO() # CustomerDTO | Customer Details

    try:
        # Edits a customer
        api_instance.update_customer(customer_id, api_version, customer_dto)
    except Exception as e:
        print("Exception when calling CustomersApi->update_customer: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customer_id** | **str**| Customer Id | 
 **api_version** | **str**| Defaults to 1 | [default to &#39;1&#39;]
 **customer_dto** | [**CustomerDTO**](CustomerDTO.md)| Customer Details | 

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

