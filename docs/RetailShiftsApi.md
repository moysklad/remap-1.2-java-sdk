# RetailShiftsApi

All URIs are relative to *https://api.moysklad.ru/api/remap/1.2*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createRetailShift**](RetailShiftsApi.md#createRetailShift) | **POST** /entity/retailshift | Создать Розничную смену |
| [**createRetailShiftBatch**](RetailShiftsApi.md#createRetailShiftBatch) | **POST** /entity/retailshift/batch | Массовое создание и обновление Розничных смен |
| [**createRetailShiftMetadataAttribute**](RetailShiftsApi.md#createRetailShiftMetadataAttribute) | **POST** /entity/retailshift/metadata/attributes | Создать доп. поле Розничной смены |
| [**deleteRetailShift**](RetailShiftsApi.md#deleteRetailShift) | **DELETE** /entity/retailshift/{id} | Удалить Розничную смену |
| [**deleteRetailShiftBatch**](RetailShiftsApi.md#deleteRetailShiftBatch) | **POST** /entity/retailshift/delete | Массовое удаление Розничных смен |
| [**deleteRetailShiftMetadataAttributeById**](RetailShiftsApi.md#deleteRetailShiftMetadataAttributeById) | **DELETE** /entity/retailshift/metadata/attributes/{id} | Удалить отдельное доп. поле Розничной смены |
| [**getRetailShiftById**](RetailShiftsApi.md#getRetailShiftById) | **GET** /entity/retailshift/{id} | Получить Розничную смену |
| [**getRetailShiftMetadata**](RetailShiftsApi.md#getRetailShiftMetadata) | **GET** /entity/retailshift/metadata | Метаданные Розничных смен |
| [**getRetailShiftMetadataAttribute**](RetailShiftsApi.md#getRetailShiftMetadataAttribute) | **GET** /entity/retailshift/metadata/attributes | Доп. поля Розничной смены |
| [**getRetailShiftMetadataAttributeById**](RetailShiftsApi.md#getRetailShiftMetadataAttributeById) | **GET** /entity/retailshift/metadata/attributes/{id} | Отдельное доп. поле Розничной смены |
| [**getRetailShifts**](RetailShiftsApi.md#getRetailShifts) | **GET** /entity/retailshift | Получить список Розничных смен |
| [**updateRetailShift**](RetailShiftsApi.md#updateRetailShift) | **PUT** /entity/retailshift/{id} | Изменить Розничную смену |
| [**updateRetailShiftMetadataAttributeById**](RetailShiftsApi.md#updateRetailShiftMetadataAttributeById) | **PUT** /entity/retailshift/metadata/attributes/{id} | Обновить отдельное доп. поле Розничной смены |



## createRetailShift

> RetailShift createRetailShift(retailShift, expand, accept, acceptEncoding, contentType)

Создать Розничную смену

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.RetailShiftsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://api.moysklad.ru/api/remap/1.2");
        
        // Configure HTTP basic authorization: basicAuth
        HttpBasicAuth basicAuth = (HttpBasicAuth) defaultClient.getAuthentication("basicAuth");
        basicAuth.setUsername("YOUR USERNAME");
        basicAuth.setPassword("YOUR PASSWORD");

        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        RetailShiftsApi apiInstance = new RetailShiftsApi(defaultClient);
        RetailShift retailShift = new RetailShift(); // RetailShift | 
        String expand = "expand_example"; // String | Замена ссылок объектами с помощью expand
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            RetailShift result = apiInstance.createRetailShift(retailShift, expand, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling RetailShiftsApi#createRetailShift");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Reason: " + e.getResponseBody());
            System.err.println("Response headers: " + e.getResponseHeaders());
            e.printStackTrace();
        }
    }
}
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **retailShift** | [**RetailShift**](RetailShift.md)|  | |
| **expand** | **String**| Замена ссылок объектами с помощью expand | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**RetailShift**](RetailShift.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## createRetailShiftBatch

> List&lt;CreateRetailShiftBatch200ResponseInner&gt; createRetailShiftBatch(retailShift, expand, accept, acceptEncoding, contentType)

Массовое создание и обновление Розничных смен

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.RetailShiftsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://api.moysklad.ru/api/remap/1.2");
        
        // Configure HTTP basic authorization: basicAuth
        HttpBasicAuth basicAuth = (HttpBasicAuth) defaultClient.getAuthentication("basicAuth");
        basicAuth.setUsername("YOUR USERNAME");
        basicAuth.setPassword("YOUR PASSWORD");

        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        RetailShiftsApi apiInstance = new RetailShiftsApi(defaultClient);
        List<RetailShift> retailShift = Arrays.asList(); // List<RetailShift> | 
        String expand = "expand_example"; // String | Замена ссылок объектами с помощью expand
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            List<CreateRetailShiftBatch200ResponseInner> result = apiInstance.createRetailShiftBatch(retailShift, expand, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling RetailShiftsApi#createRetailShiftBatch");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Reason: " + e.getResponseBody());
            System.err.println("Response headers: " + e.getResponseHeaders());
            e.printStackTrace();
        }
    }
}
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **retailShift** | [**List&lt;RetailShift&gt;**](RetailShift.md)|  | |
| **expand** | **String**| Замена ссылок объектами с помощью expand | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**List&lt;CreateRetailShiftBatch200ResponseInner&gt;**](CreateRetailShiftBatch200ResponseInner.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## createRetailShiftMetadataAttribute

> AttributeMetaInfo createRetailShiftMetadataAttribute(attributeMetaInfo, accept, acceptEncoding, contentType)

Создать доп. поле Розничной смены

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.RetailShiftsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://api.moysklad.ru/api/remap/1.2");
        
        // Configure HTTP basic authorization: basicAuth
        HttpBasicAuth basicAuth = (HttpBasicAuth) defaultClient.getAuthentication("basicAuth");
        basicAuth.setUsername("YOUR USERNAME");
        basicAuth.setPassword("YOUR PASSWORD");

        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        RetailShiftsApi apiInstance = new RetailShiftsApi(defaultClient);
        AttributeMetaInfo attributeMetaInfo = new AttributeMetaInfo(); // AttributeMetaInfo | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            AttributeMetaInfo result = apiInstance.createRetailShiftMetadataAttribute(attributeMetaInfo, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling RetailShiftsApi#createRetailShiftMetadataAttribute");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Reason: " + e.getResponseBody());
            System.err.println("Response headers: " + e.getResponseHeaders());
            e.printStackTrace();
        }
    }
}
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **attributeMetaInfo** | [**AttributeMetaInfo**](AttributeMetaInfo.md)|  | |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**AttributeMetaInfo**](AttributeMetaInfo.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## deleteRetailShift

> deleteRetailShift(id, accept, acceptEncoding)

Удалить Розничную смену

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.RetailShiftsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://api.moysklad.ru/api/remap/1.2");
        
        // Configure HTTP basic authorization: basicAuth
        HttpBasicAuth basicAuth = (HttpBasicAuth) defaultClient.getAuthentication("basicAuth");
        basicAuth.setUsername("YOUR USERNAME");
        basicAuth.setPassword("YOUR PASSWORD");

        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        RetailShiftsApi apiInstance = new RetailShiftsApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            apiInstance.deleteRetailShift(id, accept, acceptEncoding);
        } catch (ApiException e) {
            System.err.println("Exception when calling RetailShiftsApi#deleteRetailShift");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Reason: " + e.getResponseBody());
            System.err.println("Response headers: " + e.getResponseHeaders());
            e.printStackTrace();
        }
    }
}
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | **UUID**| ID сущности | |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |

### Return type

null (empty response body)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## deleteRetailShiftBatch

> List&lt;DeleteInvoiceOutBatch200ResponseInner&gt; deleteRetailShiftBatch(retailShift, accept, acceptEncoding, contentType)

Массовое удаление Розничных смен

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.RetailShiftsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://api.moysklad.ru/api/remap/1.2");
        
        // Configure HTTP basic authorization: basicAuth
        HttpBasicAuth basicAuth = (HttpBasicAuth) defaultClient.getAuthentication("basicAuth");
        basicAuth.setUsername("YOUR USERNAME");
        basicAuth.setPassword("YOUR PASSWORD");

        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        RetailShiftsApi apiInstance = new RetailShiftsApi(defaultClient);
        List<RetailShift> retailShift = Arrays.asList(); // List<RetailShift> | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            List<DeleteInvoiceOutBatch200ResponseInner> result = apiInstance.deleteRetailShiftBatch(retailShift, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling RetailShiftsApi#deleteRetailShiftBatch");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Reason: " + e.getResponseBody());
            System.err.println("Response headers: " + e.getResponseHeaders());
            e.printStackTrace();
        }
    }
}
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **retailShift** | [**List&lt;RetailShift&gt;**](RetailShift.md)|  | |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**List&lt;DeleteInvoiceOutBatch200ResponseInner&gt;**](DeleteInvoiceOutBatch200ResponseInner.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Результат по каждому элементу (успех или объект ошибки) |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## deleteRetailShiftMetadataAttributeById

> deleteRetailShiftMetadataAttributeById(id, accept, acceptEncoding)

Удалить отдельное доп. поле Розничной смены

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.RetailShiftsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://api.moysklad.ru/api/remap/1.2");
        
        // Configure HTTP basic authorization: basicAuth
        HttpBasicAuth basicAuth = (HttpBasicAuth) defaultClient.getAuthentication("basicAuth");
        basicAuth.setUsername("YOUR USERNAME");
        basicAuth.setPassword("YOUR PASSWORD");

        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        RetailShiftsApi apiInstance = new RetailShiftsApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            apiInstance.deleteRetailShiftMetadataAttributeById(id, accept, acceptEncoding);
        } catch (ApiException e) {
            System.err.println("Exception when calling RetailShiftsApi#deleteRetailShiftMetadataAttributeById");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Reason: " + e.getResponseBody());
            System.err.println("Response headers: " + e.getResponseHeaders());
            e.printStackTrace();
        }
    }
}
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | **UUID**| ID сущности | |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |

### Return type

null (empty response body)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## getRetailShiftById

> RetailShift getRetailShiftById(id, expand, accept, acceptEncoding)

Получить Розничную смену

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.RetailShiftsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://api.moysklad.ru/api/remap/1.2");
        
        // Configure HTTP basic authorization: basicAuth
        HttpBasicAuth basicAuth = (HttpBasicAuth) defaultClient.getAuthentication("basicAuth");
        basicAuth.setUsername("YOUR USERNAME");
        basicAuth.setPassword("YOUR PASSWORD");

        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        RetailShiftsApi apiInstance = new RetailShiftsApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        String expand = "expand_example"; // String | Замена ссылок объектами с помощью expand
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            RetailShift result = apiInstance.getRetailShiftById(id, expand, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling RetailShiftsApi#getRetailShiftById");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Reason: " + e.getResponseBody());
            System.err.println("Response headers: " + e.getResponseHeaders());
            e.printStackTrace();
        }
    }
}
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | **UUID**| ID сущности | |
| **expand** | **String**| Замена ссылок объектами с помощью expand | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |

### Return type

[**RetailShift**](RetailShift.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## getRetailShiftMetadata

> DocumentMetadata getRetailShiftMetadata(accept, acceptEncoding)

Метаданные Розничных смен

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.RetailShiftsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://api.moysklad.ru/api/remap/1.2");
        
        // Configure HTTP basic authorization: basicAuth
        HttpBasicAuth basicAuth = (HttpBasicAuth) defaultClient.getAuthentication("basicAuth");
        basicAuth.setUsername("YOUR USERNAME");
        basicAuth.setPassword("YOUR PASSWORD");

        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        RetailShiftsApi apiInstance = new RetailShiftsApi(defaultClient);
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            DocumentMetadata result = apiInstance.getRetailShiftMetadata(accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling RetailShiftsApi#getRetailShiftMetadata");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Reason: " + e.getResponseBody());
            System.err.println("Response headers: " + e.getResponseHeaders());
            e.printStackTrace();
        }
    }
}
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |

### Return type

[**DocumentMetadata**](DocumentMetadata.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## getRetailShiftMetadataAttribute

> AttributeMetaInfoList getRetailShiftMetadataAttribute(offset, limit, accept, acceptEncoding)

Доп. поля Розничной смены

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.RetailShiftsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://api.moysklad.ru/api/remap/1.2");
        
        // Configure HTTP basic authorization: basicAuth
        HttpBasicAuth basicAuth = (HttpBasicAuth) defaultClient.getAuthentication("basicAuth");
        basicAuth.setUsername("YOUR USERNAME");
        basicAuth.setPassword("YOUR PASSWORD");

        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        RetailShiftsApi apiInstance = new RetailShiftsApi(defaultClient);
        Integer offset = 0; // Integer | Отступ в выданном списке
        Integer limit = 1000; // Integer | Максимальное количество элементов в выданном списке (максимум 1000)
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            AttributeMetaInfoList result = apiInstance.getRetailShiftMetadataAttribute(offset, limit, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling RetailShiftsApi#getRetailShiftMetadataAttribute");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Reason: " + e.getResponseBody());
            System.err.println("Response headers: " + e.getResponseHeaders());
            e.printStackTrace();
        }
    }
}
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **offset** | **Integer**| Отступ в выданном списке | [optional] [default to 0] |
| **limit** | **Integer**| Максимальное количество элементов в выданном списке (максимум 1000) | [optional] [default to 1000] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |

### Return type

[**AttributeMetaInfoList**](AttributeMetaInfoList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## getRetailShiftMetadataAttributeById

> AttributeMetaInfo getRetailShiftMetadataAttributeById(id, accept, acceptEncoding)

Отдельное доп. поле Розничной смены

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.RetailShiftsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://api.moysklad.ru/api/remap/1.2");
        
        // Configure HTTP basic authorization: basicAuth
        HttpBasicAuth basicAuth = (HttpBasicAuth) defaultClient.getAuthentication("basicAuth");
        basicAuth.setUsername("YOUR USERNAME");
        basicAuth.setPassword("YOUR PASSWORD");

        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        RetailShiftsApi apiInstance = new RetailShiftsApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            AttributeMetaInfo result = apiInstance.getRetailShiftMetadataAttributeById(id, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling RetailShiftsApi#getRetailShiftMetadataAttributeById");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Reason: " + e.getResponseBody());
            System.err.println("Response headers: " + e.getResponseHeaders());
            e.printStackTrace();
        }
    }
}
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | **UUID**| ID сущности | |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |

### Return type

[**AttributeMetaInfo**](AttributeMetaInfo.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## getRetailShifts

> RetailShiftList getRetailShifts(limit, offset, expand, accept, acceptEncoding)

Получить список Розничных смен

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.RetailShiftsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://api.moysklad.ru/api/remap/1.2");
        
        // Configure HTTP basic authorization: basicAuth
        HttpBasicAuth basicAuth = (HttpBasicAuth) defaultClient.getAuthentication("basicAuth");
        basicAuth.setUsername("YOUR USERNAME");
        basicAuth.setPassword("YOUR PASSWORD");

        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        RetailShiftsApi apiInstance = new RetailShiftsApi(defaultClient);
        Integer limit = 1000; // Integer | Максимальное количество элементов в выданном списке (максимум 1000)
        Integer offset = 0; // Integer | Отступ в выданном списке
        String expand = "expand_example"; // String | Замена ссылок объектами с помощью expand
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            RetailShiftList result = apiInstance.getRetailShifts(limit, offset, expand, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling RetailShiftsApi#getRetailShifts");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Reason: " + e.getResponseBody());
            System.err.println("Response headers: " + e.getResponseHeaders());
            e.printStackTrace();
        }
    }
}
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **limit** | **Integer**| Максимальное количество элементов в выданном списке (максимум 1000) | [optional] [default to 1000] |
| **offset** | **Integer**| Отступ в выданном списке | [optional] [default to 0] |
| **expand** | **String**| Замена ссылок объектами с помощью expand | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |

### Return type

[**RetailShiftList**](RetailShiftList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## updateRetailShift

> RetailShift updateRetailShift(id, retailShift, expand, accept, acceptEncoding, contentType)

Изменить Розничную смену

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.RetailShiftsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://api.moysklad.ru/api/remap/1.2");
        
        // Configure HTTP basic authorization: basicAuth
        HttpBasicAuth basicAuth = (HttpBasicAuth) defaultClient.getAuthentication("basicAuth");
        basicAuth.setUsername("YOUR USERNAME");
        basicAuth.setPassword("YOUR PASSWORD");

        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        RetailShiftsApi apiInstance = new RetailShiftsApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        RetailShift retailShift = new RetailShift(); // RetailShift | 
        String expand = "expand_example"; // String | Замена ссылок объектами с помощью expand
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            RetailShift result = apiInstance.updateRetailShift(id, retailShift, expand, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling RetailShiftsApi#updateRetailShift");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Reason: " + e.getResponseBody());
            System.err.println("Response headers: " + e.getResponseHeaders());
            e.printStackTrace();
        }
    }
}
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | **UUID**| ID сущности | |
| **retailShift** | [**RetailShift**](RetailShift.md)|  | |
| **expand** | **String**| Замена ссылок объектами с помощью expand | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**RetailShift**](RetailShift.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## updateRetailShiftMetadataAttributeById

> AttributeMetaInfo updateRetailShiftMetadataAttributeById(id, attributeMetaInfo, accept, acceptEncoding, contentType)

Обновить отдельное доп. поле Розничной смены

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.RetailShiftsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://api.moysklad.ru/api/remap/1.2");
        
        // Configure HTTP basic authorization: basicAuth
        HttpBasicAuth basicAuth = (HttpBasicAuth) defaultClient.getAuthentication("basicAuth");
        basicAuth.setUsername("YOUR USERNAME");
        basicAuth.setPassword("YOUR PASSWORD");

        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        RetailShiftsApi apiInstance = new RetailShiftsApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        AttributeMetaInfo attributeMetaInfo = new AttributeMetaInfo(); // AttributeMetaInfo | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            AttributeMetaInfo result = apiInstance.updateRetailShiftMetadataAttributeById(id, attributeMetaInfo, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling RetailShiftsApi#updateRetailShiftMetadataAttributeById");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Reason: " + e.getResponseBody());
            System.err.println("Response headers: " + e.getResponseHeaders());
            e.printStackTrace();
        }
    }
}
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | **UUID**| ID сущности | |
| **attributeMetaInfo** | [**AttributeMetaInfo**](AttributeMetaInfo.md)|  | |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**AttributeMetaInfo**](AttributeMetaInfo.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |

