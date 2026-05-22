# LabelsApi

All URIs are relative to *https://api.moysklad.ru/api/remap/1.2*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**printLabels**](LabelsApi.md#printLabels) | **POST** /entity/{type}/{id}/export | Запрос на печать этикеток и ценников |



## printLabels

> printLabels(id, type, labelPrintRequest, accept, acceptEncoding, contentType)

Запрос на печать этикеток и ценников

Запрос на формирование печатной формы с этикетками и ценниками. В случае готовности сервер возвращает пустой ответ с кодом 303 и заголовком Location. 

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.LabelsApi;

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

        LabelsApi apiInstance = new LabelsApi(defaultClient);
        UUID id = UUID.fromString("12a8b923-692c-11e6-8a84-bae500000053"); // UUID | ID сущности
        String type = "product"; // String | Тип сущности, для которой запрашивается печать
        LabelPrintRequest labelPrintRequest = new LabelPrintRequest(); // LabelPrintRequest | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            apiInstance.printLabels(id, type, labelPrintRequest, accept, acceptEncoding, contentType);
        } catch (ApiException e) {
            System.err.println("Exception when calling LabelsApi#printLabels");
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
| **type** | **String**| Тип сущности, для которой запрашивается печать | [enum: product, service, bundle, variant] |
| **labelPrintRequest** | [**LabelPrintRequest**](LabelPrintRequest.md)|  | |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

null (empty response body)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **202** | Печатная форма еще не готова, в Location передана ссылка на статус печати |  * Location - Ссылка на статус печати <br>  * Content-Type - Тип содержимого ответа <br>  |
| **303** | Печатная форма готова, в Location передана ссылка на файл |  * Location - Ссылка на статус печати <br>  * Content-Type - Тип содержимого ответа <br>  |
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

