# FactureInsApi

All URIs are relative to *https://api.moysklad.ru/api/remap/1.2*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createFactureIn**](FactureInsApi.md#createFactureIn) | **POST** /entity/facturein | Создать Счет-фактуру полученный |
| [**createFactureInMetadataAttribute**](FactureInsApi.md#createFactureInMetadataAttribute) | **POST** /entity/facturein/metadata/attributes | Создать доп. поле Счета-фактуры полученного |
| [**createFactureInMetadataState**](FactureInsApi.md#createFactureInMetadataState) | **POST** /entity/facturein/metadata/states | Создать статус Счета-фактуры полученного |
| [**createFactureInsBatch**](FactureInsApi.md#createFactureInsBatch) | **POST** /entity/facturein/batch | Массовое создание и обновление Счетов-фактур полученных |
| [**deleteFactureIn**](FactureInsApi.md#deleteFactureIn) | **DELETE** /entity/facturein/{id} | Удалить Счет-фактуру полученный |
| [**deleteFactureInMetadataAttributeById**](FactureInsApi.md#deleteFactureInMetadataAttributeById) | **DELETE** /entity/facturein/metadata/attributes/{id} | Удалить отдельное доп. поле Счета-фактуры полученного |
| [**deleteFactureInMetadataStateById**](FactureInsApi.md#deleteFactureInMetadataStateById) | **DELETE** /entity/facturein/metadata/states/{id} | Удалить отдельный статус Счета-фактуры полученного |
| [**deleteFactureInsBatch**](FactureInsApi.md#deleteFactureInsBatch) | **POST** /entity/facturein/delete | Массовое удаление Счетов-фактур полученных |
| [**getFactureInById**](FactureInsApi.md#getFactureInById) | **GET** /entity/facturein/{id} | Получить Счет-фактуру полученный |
| [**getFactureInMetadata**](FactureInsApi.md#getFactureInMetadata) | **GET** /entity/facturein/metadata | Метаданные Счетов-фактур полученных |
| [**getFactureInMetadataAttributeById**](FactureInsApi.md#getFactureInMetadataAttributeById) | **GET** /entity/facturein/metadata/attributes/{id} | Отдельное доп. поле Счета-фактуры полученного |
| [**getFactureInMetadataAttributes**](FactureInsApi.md#getFactureInMetadataAttributes) | **GET** /entity/facturein/metadata/attributes | Доп. поля Счетов-фактур полученных |
| [**getFactureInMetadataStateById**](FactureInsApi.md#getFactureInMetadataStateById) | **GET** /entity/facturein/metadata/states/{id} | Отдельный статус Счета-фактуры полученного |
| [**getFactureInTemplate**](FactureInsApi.md#getFactureInTemplate) | **PUT** /entity/facturein/new | Шаблон Счета-фактуры полученного |
| [**getFactureIns**](FactureInsApi.md#getFactureIns) | **GET** /entity/facturein | Получить список Счетов-фактур полученных |
| [**updateFactureIn**](FactureInsApi.md#updateFactureIn) | **PUT** /entity/facturein/{id} | Изменить Счет-фактуру полученный |
| [**updateFactureInMetadataAttributeById**](FactureInsApi.md#updateFactureInMetadataAttributeById) | **PUT** /entity/facturein/metadata/attributes/{id} | Обновить отдельное доп. поле Счета-фактуры полученного |
| [**updateFactureInMetadataStateById**](FactureInsApi.md#updateFactureInMetadataStateById) | **PUT** /entity/facturein/metadata/states/{id} | Обновить отдельный статус Счета-фактуры полученного |



## createFactureIn

> FactureIn createFactureIn(factureIn, expand, accept, acceptEncoding, contentType)

Создать Счет-фактуру полученный

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.FactureInsApi;

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

        FactureInsApi apiInstance = new FactureInsApi(defaultClient);
        FactureIn factureIn = new FactureIn(); // FactureIn | 
        String expand = "agent,organization"; // String | Замена ссылок объектами с помощью expand
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            FactureIn result = apiInstance.createFactureIn(factureIn, expand, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling FactureInsApi#createFactureIn");
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
| **factureIn** | [**FactureIn**](FactureIn.md)|  | |
| **expand** | **String**| Замена ссылок объектами с помощью expand | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**FactureIn**](FactureIn.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Счет-фактура полученный успешно создан |  -  |
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |


## createFactureInMetadataAttribute

> AttributeMetaInfo createFactureInMetadataAttribute(attributeMetaInfo, accept, acceptEncoding, contentType)

Создать доп. поле Счета-фактуры полученного

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.FactureInsApi;

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

        FactureInsApi apiInstance = new FactureInsApi(defaultClient);
        AttributeMetaInfo attributeMetaInfo = new AttributeMetaInfo(); // AttributeMetaInfo | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            AttributeMetaInfo result = apiInstance.createFactureInMetadataAttribute(attributeMetaInfo, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling FactureInsApi#createFactureInMetadataAttribute");
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
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |


## createFactureInMetadataState

> State createFactureInMetadataState(state, accept, acceptEncoding, contentType)

Создать статус Счета-фактуры полученного

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.FactureInsApi;

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

        FactureInsApi apiInstance = new FactureInsApi(defaultClient);
        State state = new State(); // State | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            State result = apiInstance.createFactureInMetadataState(state, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling FactureInsApi#createFactureInMetadataState");
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
| **state** | [**State**](State.md)|  | |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**State**](State.md)

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


## createFactureInsBatch

> List&lt;CreateFactureInsBatch200ResponseInner&gt; createFactureInsBatch(factureIn, expand, accept, acceptEncoding, contentType)

Массовое создание и обновление Счетов-фактур полученных

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.FactureInsApi;

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

        FactureInsApi apiInstance = new FactureInsApi(defaultClient);
        List<FactureIn> factureIn = Arrays.asList(); // List<FactureIn> | 
        String expand = "agent,organization"; // String | Замена ссылок объектами с помощью expand
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            List<CreateFactureInsBatch200ResponseInner> result = apiInstance.createFactureInsBatch(factureIn, expand, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling FactureInsApi#createFactureInsBatch");
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
| **factureIn** | [**List&lt;FactureIn&gt;**](FactureIn.md)|  | |
| **expand** | **String**| Замена ссылок объектами с помощью expand | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**List&lt;CreateFactureInsBatch200ResponseInner&gt;**](CreateFactureInsBatch200ResponseInner.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Счета-фактуры полученные успешно созданы или изменены |  -  |
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |


## deleteFactureIn

> deleteFactureIn(id, accept, acceptEncoding)

Удалить Счет-фактуру полученный

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.FactureInsApi;

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

        FactureInsApi apiInstance = new FactureInsApi(defaultClient);
        UUID id = UUID.fromString("12a8b923-692c-11e6-8a84-bae500000053"); // UUID | ID сущности
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            apiInstance.deleteFactureIn(id, accept, acceptEncoding);
        } catch (ApiException e) {
            System.err.println("Exception when calling FactureInsApi#deleteFactureIn");
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
| **200** | Счет-фактура полученный успешно удалена |  -  |
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |


## deleteFactureInMetadataAttributeById

> deleteFactureInMetadataAttributeById(id, accept, acceptEncoding)

Удалить отдельное доп. поле Счета-фактуры полученного

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.FactureInsApi;

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

        FactureInsApi apiInstance = new FactureInsApi(defaultClient);
        UUID id = UUID.fromString("12a8b923-692c-11e6-8a84-bae500000053"); // UUID | ID сущности
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            apiInstance.deleteFactureInMetadataAttributeById(id, accept, acceptEncoding);
        } catch (ApiException e) {
            System.err.println("Exception when calling FactureInsApi#deleteFactureInMetadataAttributeById");
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
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |


## deleteFactureInMetadataStateById

> deleteFactureInMetadataStateById(id, accept, acceptEncoding)

Удалить отдельный статус Счета-фактуры полученного

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.FactureInsApi;

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

        FactureInsApi apiInstance = new FactureInsApi(defaultClient);
        UUID id = UUID.fromString("12a8b923-692c-11e6-8a84-bae500000053"); // UUID | ID сущности
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            apiInstance.deleteFactureInMetadataStateById(id, accept, acceptEncoding);
        } catch (ApiException e) {
            System.err.println("Exception when calling FactureInsApi#deleteFactureInMetadataStateById");
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
| **404** | Запрошенный ресурс не существует (тело ответа отсутствует) |  -  |
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |


## deleteFactureInsBatch

> List&lt;DeleteContractsBatch200ResponseInner&gt; deleteFactureInsBatch(factureIn, accept, acceptEncoding, contentType)

Массовое удаление Счетов-фактур полученных

Массовое удаление Счетов-фактур полученных по их мета-объектам

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.FactureInsApi;

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

        FactureInsApi apiInstance = new FactureInsApi(defaultClient);
        List<FactureIn> factureIn = Arrays.asList(); // List<FactureIn> | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            List<DeleteContractsBatch200ResponseInner> result = apiInstance.deleteFactureInsBatch(factureIn, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling FactureInsApi#deleteFactureInsBatch");
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
| **factureIn** | [**List&lt;FactureIn&gt;**](FactureIn.md)|  | |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**List&lt;DeleteContractsBatch200ResponseInner&gt;**](DeleteContractsBatch200ResponseInner.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Результат по каждому элементу (успех или объект ошибки) |  -  |
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |


## getFactureInById

> FactureIn getFactureInById(id, expand, accept, acceptEncoding)

Получить Счет-фактуру полученный

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.FactureInsApi;

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

        FactureInsApi apiInstance = new FactureInsApi(defaultClient);
        UUID id = UUID.fromString("12a8b923-692c-11e6-8a84-bae500000053"); // UUID | ID сущности
        String expand = "agent,organization"; // String | Замена ссылок объектами с помощью expand
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            FactureIn result = apiInstance.getFactureInById(id, expand, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling FactureInsApi#getFactureInById");
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

[**FactureIn**](FactureIn.md)

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


## getFactureInMetadata

> DocumentMetadata getFactureInMetadata(expand, accept, acceptEncoding)

Метаданные Счетов-фактур полученных

Запрос на получение метаданных Счетов-фактур полученных

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.FactureInsApi;

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

        FactureInsApi apiInstance = new FactureInsApi(defaultClient);
        String expand = "agent,organization"; // String | Замена ссылок объектами с помощью expand
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            DocumentMetadata result = apiInstance.getFactureInMetadata(expand, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling FactureInsApi#getFactureInMetadata");
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
| **expand** | **String**| Замена ссылок объектами с помощью expand | [optional] |
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
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |


## getFactureInMetadataAttributeById

> AttributeMetaInfo getFactureInMetadataAttributeById(id, accept, acceptEncoding)

Отдельное доп. поле Счета-фактуры полученного

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.FactureInsApi;

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

        FactureInsApi apiInstance = new FactureInsApi(defaultClient);
        UUID id = UUID.fromString("12a8b923-692c-11e6-8a84-bae500000053"); // UUID | ID сущности
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            AttributeMetaInfo result = apiInstance.getFactureInMetadataAttributeById(id, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling FactureInsApi#getFactureInMetadataAttributeById");
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
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |


## getFactureInMetadataAttributes

> AttributeMetaInfoList getFactureInMetadataAttributes(offset, limit, accept, acceptEncoding)

Доп. поля Счетов-фактур полученных

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.FactureInsApi;

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

        FactureInsApi apiInstance = new FactureInsApi(defaultClient);
        Integer offset = 0; // Integer | Отступ в выданном списке
        Integer limit = 1000; // Integer | Максимальное количество элементов в выданном списке (максимум 1000)
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            AttributeMetaInfoList result = apiInstance.getFactureInMetadataAttributes(offset, limit, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling FactureInsApi#getFactureInMetadataAttributes");
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
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |


## getFactureInMetadataStateById

> State getFactureInMetadataStateById(id, accept, acceptEncoding)

Отдельный статус Счета-фактуры полученного

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.FactureInsApi;

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

        FactureInsApi apiInstance = new FactureInsApi(defaultClient);
        UUID id = UUID.fromString("12a8b923-692c-11e6-8a84-bae500000053"); // UUID | ID сущности
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            State result = apiInstance.getFactureInMetadataStateById(id, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling FactureInsApi#getFactureInMetadataStateById");
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

[**State**](State.md)

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


## getFactureInTemplate

> FactureIn getFactureInTemplate(body, accept, acceptEncoding, contentType)

Шаблон Счета-фактуры полученного

Предзаполненный шаблон Счета-фактуры полученного на основе приемки или исходящего платежа. 

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.FactureInsApi;

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

        FactureInsApi apiInstance = new FactureInsApi(defaultClient);
        Object body = null; // Object | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            FactureIn result = apiInstance.getFactureInTemplate(body, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling FactureInsApi#getFactureInTemplate");
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
| **body** | **Object**|  | |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**FactureIn**](FactureIn.md)

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


## getFactureIns

> FactureInList getFactureIns(limit, offset, search, filter, expand, order, accept, acceptEncoding)

Получить список Счетов-фактур полученных

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.FactureInsApi;

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

        FactureInsApi apiInstance = new FactureInsApi(defaultClient);
        Integer limit = 1000; // Integer | Максимальное количество элементов в выданном списке (максимум 1000)
        Integer offset = 0; // Integer | Отступ в выданном списке
        String search = "name=123"; // String | Контекстный поиск по строковым полям сущностей
        String filter = "archived=false"; // String | Фильтрация выборки
        String expand = "agent,organization"; // String | Замена ссылок объектами с помощью expand
        String order = "name"; // String | Сортировка
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            FactureInList result = apiInstance.getFactureIns(limit, offset, search, filter, expand, order, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling FactureInsApi#getFactureIns");
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
| **search** | **String**| Контекстный поиск по строковым полям сущностей | [optional] |
| **filter** | **String**| Фильтрация выборки | [optional] |
| **expand** | **String**| Замена ссылок объектами с помощью expand | [optional] |
| **order** | **String**| Сортировка | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |

### Return type

[**FactureInList**](FactureInList.md)

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


## updateFactureIn

> FactureIn updateFactureIn(id, factureIn, expand, accept, acceptEncoding, contentType)

Изменить Счет-фактуру полученный

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.FactureInsApi;

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

        FactureInsApi apiInstance = new FactureInsApi(defaultClient);
        UUID id = UUID.fromString("12a8b923-692c-11e6-8a84-bae500000053"); // UUID | ID сущности
        FactureIn factureIn = new FactureIn(); // FactureIn | 
        String expand = "agent,organization"; // String | Замена ссылок объектами с помощью expand
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            FactureIn result = apiInstance.updateFactureIn(id, factureIn, expand, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling FactureInsApi#updateFactureIn");
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
| **factureIn** | [**FactureIn**](FactureIn.md)|  | |
| **expand** | **String**| Замена ссылок объектами с помощью expand | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**FactureIn**](FactureIn.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Счет-фактура полученный успешно обновлен |  -  |
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |


## updateFactureInMetadataAttributeById

> AttributeMetaInfo updateFactureInMetadataAttributeById(id, attributeMetaInfo, accept, acceptEncoding, contentType)

Обновить отдельное доп. поле Счета-фактуры полученного

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.FactureInsApi;

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

        FactureInsApi apiInstance = new FactureInsApi(defaultClient);
        UUID id = UUID.fromString("12a8b923-692c-11e6-8a84-bae500000053"); // UUID | ID сущности
        AttributeMetaInfo attributeMetaInfo = new AttributeMetaInfo(); // AttributeMetaInfo | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            AttributeMetaInfo result = apiInstance.updateFactureInMetadataAttributeById(id, attributeMetaInfo, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling FactureInsApi#updateFactureInMetadataAttributeById");
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
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |


## updateFactureInMetadataStateById

> State updateFactureInMetadataStateById(id, state, accept, acceptEncoding, contentType)

Обновить отдельный статус Счета-фактуры полученного

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.FactureInsApi;

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

        FactureInsApi apiInstance = new FactureInsApi(defaultClient);
        UUID id = UUID.fromString("12a8b923-692c-11e6-8a84-bae500000053"); // UUID | ID сущности
        State state = new State(); // State | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            State result = apiInstance.updateFactureInMetadataStateById(id, state, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling FactureInsApi#updateFactureInMetadataStateById");
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
| **state** | [**State**](State.md)|  | |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**State**](State.md)

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

