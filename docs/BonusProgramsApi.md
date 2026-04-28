# BonusProgramsApi

All URIs are relative to *https://api.moysklad.ru/api/remap/1.2*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createBonusProgram**](BonusProgramsApi.md#createBonusProgram) | **POST** /entity/bonusprogram | Создать бонусную программу |
| [**deleteBonusProgram**](BonusProgramsApi.md#deleteBonusProgram) | **DELETE** /entity/bonusprogram/{id} | Удалить бонусную программу |
| [**deleteBonusProgramsBatch**](BonusProgramsApi.md#deleteBonusProgramsBatch) | **POST** /entity/bonusprogram/delete | Удалить бонусные программы |
| [**getBonusProgramById**](BonusProgramsApi.md#getBonusProgramById) | **GET** /entity/bonusprogram/{id} | Получить бонусную программу по ID |
| [**getBonusPrograms**](BonusProgramsApi.md#getBonusPrograms) | **GET** /entity/bonusprogram | Получить список бонусных программ |
| [**updateBonusProgram**](BonusProgramsApi.md#updateBonusProgram) | **PUT** /entity/bonusprogram/{id} | Изменить бонусную программу |



## createBonusProgram

> BonusProgram createBonusProgram(bonusProgram, expand, accept, acceptEncoding, contentType)

Создать бонусную программу

Создание новой бонусной программы

### Example

```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.BonusProgramsApi;

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

        BonusProgramsApi apiInstance = new BonusProgramsApi(defaultClient);
        BonusProgram bonusProgram = new BonusProgram(); // BonusProgram | 
        String expand = "agent,organization"; // String | Замена ссылок объектами с помощью expand
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            BonusProgram result = apiInstance.createBonusProgram(bonusProgram, expand, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling BonusProgramsApi#createBonusProgram");
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
| **bonusProgram** | [**BonusProgram**](BonusProgram.md)|  | |
| **expand** | **String**| Замена ссылок объектами с помощью expand | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**BonusProgram**](BonusProgram.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Бонусная программа успешно создана |  -  |
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |


## deleteBonusProgram

> deleteBonusProgram(id, accept, acceptEncoding)

Удалить бонусную программу

Удаление бонусной программы с указанным id

### Example

```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.BonusProgramsApi;

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

        BonusProgramsApi apiInstance = new BonusProgramsApi(defaultClient);
        UUID id = UUID.fromString("12a8b923-692c-11e6-8a84-bae500000053"); // UUID | ID сущности
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            apiInstance.deleteBonusProgram(id, accept, acceptEncoding);
        } catch (ApiException e) {
            System.err.println("Exception when calling BonusProgramsApi#deleteBonusProgram");
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
| **200** | Бонусная программа успешно удалена |  -  |
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |


## deleteBonusProgramsBatch

> List&lt;DeleteContractsBatch200ResponseInner&gt; deleteBonusProgramsBatch(bonusProgram, accept, acceptEncoding, contentType)

Удалить бонусные программы

Массовое удаление бонусных программ по их мета-объектам.

### Example

```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.BonusProgramsApi;

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

        BonusProgramsApi apiInstance = new BonusProgramsApi(defaultClient);
        List<BonusProgram> bonusProgram = Arrays.asList(); // List<BonusProgram> | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            List<DeleteContractsBatch200ResponseInner> result = apiInstance.deleteBonusProgramsBatch(bonusProgram, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling BonusProgramsApi#deleteBonusProgramsBatch");
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
| **bonusProgram** | [**List&lt;BonusProgram&gt;**](BonusProgram.md)|  | |
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


## getBonusProgramById

> BonusProgram getBonusProgramById(id, expand, accept, acceptEncoding)

Получить бонусную программу по ID

Запрос бонусной программы с указанным id

### Example

```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.BonusProgramsApi;

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

        BonusProgramsApi apiInstance = new BonusProgramsApi(defaultClient);
        UUID id = UUID.fromString("12a8b923-692c-11e6-8a84-bae500000053"); // UUID | ID сущности
        String expand = "agent,organization"; // String | Замена ссылок объектами с помощью expand
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            BonusProgram result = apiInstance.getBonusProgramById(id, expand, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling BonusProgramsApi#getBonusProgramById");
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

[**BonusProgram**](BonusProgram.md)

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


## getBonusPrograms

> BonusProgramList getBonusPrograms(limit, offset, search, filter, expand, order, accept, acceptEncoding)

Получить список бонусных программ

Запрос всех бонусных программ на данной учетной записи

### Example

```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.BonusProgramsApi;

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

        BonusProgramsApi apiInstance = new BonusProgramsApi(defaultClient);
        Integer limit = 1000; // Integer | Максимальное количество элементов в выданном списке (максимум 1000)
        Integer offset = 0; // Integer | Отступ в выданном списке
        String search = "name=123"; // String | Контекстный поиск по строковым полям сущностей
        String filter = "archived=false"; // String | Фильтрация выборки
        String expand = "agent,organization"; // String | Замена ссылок объектами с помощью expand
        String order = "name"; // String | Сортировка
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            BonusProgramList result = apiInstance.getBonusPrograms(limit, offset, search, filter, expand, order, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling BonusProgramsApi#getBonusPrograms");
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

[**BonusProgramList**](BonusProgramList.md)

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


## updateBonusProgram

> BonusProgram updateBonusProgram(id, bonusProgram, expand, accept, acceptEncoding, contentType)

Изменить бонусную программу

Запрос на изменение бонусной программы с указанным id

### Example

```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.BonusProgramsApi;

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

        BonusProgramsApi apiInstance = new BonusProgramsApi(defaultClient);
        UUID id = UUID.fromString("12a8b923-692c-11e6-8a84-bae500000053"); // UUID | ID сущности
        BonusProgram bonusProgram = new BonusProgram(); // BonusProgram | 
        String expand = "agent,organization"; // String | Замена ссылок объектами с помощью expand
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            BonusProgram result = apiInstance.updateBonusProgram(id, bonusProgram, expand, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling BonusProgramsApi#updateBonusProgram");
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
| **bonusProgram** | [**BonusProgram**](BonusProgram.md)|  | |
| **expand** | **String**| Замена ссылок объектами с помощью expand | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**BonusProgram**](BonusProgram.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Бонусная программа успешно обновлена |  -  |
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

