# VariantCharacteristicsApi

All URIs are relative to *https://api.moysklad.ru/api/remap/1.2*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createVariantCharacteristic**](VariantCharacteristicsApi.md#createVariantCharacteristic) | **POST** /entity/variant/metadata/characteristics | Создать Характеристику модификаций |
| [**getVariantCharacteristicById**](VariantCharacteristicsApi.md#getVariantCharacteristicById) | **GET** /entity/variant/metadata/characteristics/{id} | Получить Характеристику модификаций |
| [**getVariantCharacteristics**](VariantCharacteristicsApi.md#getVariantCharacteristics) | **GET** /entity/variant/metadata/characteristics | Получить список Характеристики модификаций |



## createVariantCharacteristic

> VariantCharacteristic createVariantCharacteristic(variantCharacteristic, accept, acceptEncoding)

Создать Характеристику модификаций

### Example

```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.VariantCharacteristicsApi;

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

        VariantCharacteristicsApi apiInstance = new VariantCharacteristicsApi(defaultClient);
        VariantCharacteristic variantCharacteristic = new VariantCharacteristic(); // VariantCharacteristic | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            VariantCharacteristic result = apiInstance.createVariantCharacteristic(variantCharacteristic, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling VariantCharacteristicsApi#createVariantCharacteristic");
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
| **variantCharacteristic** | [**VariantCharacteristic**](VariantCharacteristic.md)|  | |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |

### Return type

[**VariantCharacteristic**](VariantCharacteristic.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос |  -  |
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |


## getVariantCharacteristicById

> VariantCharacteristic getVariantCharacteristicById(id, accept, acceptEncoding)

Получить Характеристику модификаций

### Example

```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.VariantCharacteristicsApi;

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

        VariantCharacteristicsApi apiInstance = new VariantCharacteristicsApi(defaultClient);
        UUID id = UUID.fromString("12a8b923-692c-11e6-8a84-bae500000053"); // UUID | ID сущности
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            VariantCharacteristic result = apiInstance.getVariantCharacteristicById(id, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling VariantCharacteristicsApi#getVariantCharacteristicById");
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

[**VariantCharacteristic**](VariantCharacteristic.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос |  -  |
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |


## getVariantCharacteristics

> GetVariantCharacteristics200Response getVariantCharacteristics(accept, acceptEncoding)

Получить список Характеристики модификаций

### Example

```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.VariantCharacteristicsApi;

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

        VariantCharacteristicsApi apiInstance = new VariantCharacteristicsApi(defaultClient);
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            GetVariantCharacteristics200Response result = apiInstance.getVariantCharacteristics(accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling VariantCharacteristicsApi#getVariantCharacteristics");
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

[**GetVariantCharacteristics200Response**](GetVariantCharacteristics200Response.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос |  -  |
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

