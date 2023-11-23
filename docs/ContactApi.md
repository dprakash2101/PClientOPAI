# openapi_client.ContactApi

All URIs are relative to *https://localhost:7207*

Method | HTTP request | Description
------------- | ------------- | -------------
[**contact_get**](ContactApi.md#contact_get) | **GET** /contact | 
[**contact_id_delete**](ContactApi.md#contact_id_delete) | **DELETE** /contact/{id} | 
[**contact_id_get**](ContactApi.md#contact_id_get) | **GET** /contact/{id} | 
[**contact_id_put**](ContactApi.md#contact_id_put) | **PUT** /contact/{id} | 
[**contact_post**](ContactApi.md#contact_post) | **POST** /contact | 


# **contact_get**
> List[Contact] contact_get()



### Example

```python
import time
import os
import openapi_client
from openapi_client.models.contact import Contact
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://localhost:7207
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://localhost:7207"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.ContactApi(api_client)

    try:
        api_response = api_instance.contact_get()
        print("The response of ContactApi->contact_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContactApi->contact_get: %s\n" % e)
```



### Parameters
This endpoint does not need any parameter.

### Return type

[**List[Contact]**](Contact.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **contact_id_delete**
> List[Contact] contact_id_delete(id)



### Example

```python
import time
import os
import openapi_client
from openapi_client.models.contact import Contact
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://localhost:7207
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://localhost:7207"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.ContactApi(api_client)
    id = 56 # int | 

    try:
        api_response = api_instance.contact_id_delete(id)
        print("The response of ContactApi->contact_id_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContactApi->contact_id_delete: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  | 

### Return type

[**List[Contact]**](Contact.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **contact_id_get**
> Contact contact_id_get(id)



### Example

```python
import time
import os
import openapi_client
from openapi_client.models.contact import Contact
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://localhost:7207
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://localhost:7207"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.ContactApi(api_client)
    id = 56 # int | 

    try:
        api_response = api_instance.contact_id_get(id)
        print("The response of ContactApi->contact_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContactApi->contact_id_get: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  | 

### Return type

[**Contact**](Contact.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **contact_id_put**
> List[Contact] contact_id_put(id, contact=contact)



### Example

```python
import time
import os
import openapi_client
from openapi_client.models.contact import Contact
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://localhost:7207
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://localhost:7207"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.ContactApi(api_client)
    id = 56 # int | 
    contact = openapi_client.Contact() # Contact |  (optional)

    try:
        api_response = api_instance.contact_id_put(id, contact=contact)
        print("The response of ContactApi->contact_id_put:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContactApi->contact_id_put: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  | 
 **contact** | [**Contact**](Contact.md)|  | [optional] 

### Return type

[**List[Contact]**](Contact.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **contact_post**
> List[Contact] contact_post(contact=contact)



### Example

```python
import time
import os
import openapi_client
from openapi_client.models.contact import Contact
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://localhost:7207
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://localhost:7207"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.ContactApi(api_client)
    contact = openapi_client.Contact() # Contact |  (optional)

    try:
        api_response = api_instance.contact_post(contact=contact)
        print("The response of ContactApi->contact_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContactApi->contact_post: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contact** | [**Contact**](Contact.md)|  | [optional] 

### Return type

[**List[Contact]**](Contact.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

