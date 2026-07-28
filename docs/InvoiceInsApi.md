# InvoiceInsApi

All URIs are relative to *https://api.moysklad.ru/api/remap/1.2*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**addInvoiceInFiles**](InvoiceInsApi.md#addInvoiceInFiles) | **POST** /entity/invoicein/{id}/files | Добавить файлы к Счету поставщику |
| [**createInvoiceIn**](InvoiceInsApi.md#createInvoiceIn) | **POST** /entity/invoicein | Создать Счет поставщику |
| [**createInvoiceInBatch**](InvoiceInsApi.md#createInvoiceInBatch) | **POST** /entity/invoicein/batch | Массовое создание и обновление Счетов поставщикам |
| [**createInvoiceInMetadataAttribute**](InvoiceInsApi.md#createInvoiceInMetadataAttribute) | **POST** /entity/invoicein/metadata/attributes | Создать Доп. поле InvoiceIn |
| [**createInvoiceInNote**](InvoiceInsApi.md#createInvoiceInNote) | **POST** /entity/invoicein/{id}/notes | Добавить Событие Счета поставщику |
| [**createInvoiceInPositions**](InvoiceInsApi.md#createInvoiceInPositions) | **POST** /entity/invoicein/{id}/positions | Создать позицию Счета поставщику |
| [**createInvoiceInPositionsBatch**](InvoiceInsApi.md#createInvoiceInPositionsBatch) | **POST** /entity/invoicein/{id}/positions/batch | Создать позиции Счета поставщику |
| [**deleteInvoiceIn**](InvoiceInsApi.md#deleteInvoiceIn) | **DELETE** /entity/invoicein/{id} | Удалить Счет поставщику |
| [**deleteInvoiceInBatch**](InvoiceInsApi.md#deleteInvoiceInBatch) | **POST** /entity/invoicein/delete | Массовое удаление Счетов поставщикам |
| [**deleteInvoiceInFile**](InvoiceInsApi.md#deleteInvoiceInFile) | **DELETE** /entity/invoicein/{id}/files/{fileId} | Удалить файл Счета поставщику |
| [**deleteInvoiceInMetadataAttributeById**](InvoiceInsApi.md#deleteInvoiceInMetadataAttributeById) | **DELETE** /entity/invoicein/metadata/attributes/{id} | Удалить отдельное доп. поле InvoiceIn |
| [**deleteInvoiceInMetadataStateById**](InvoiceInsApi.md#deleteInvoiceInMetadataStateById) | **DELETE** /entity/invoicein/metadata/states/{id} | Удалить отдельный статус InvoiceIn |
| [**deleteInvoiceInNote**](InvoiceInsApi.md#deleteInvoiceInNote) | **DELETE** /entity/invoicein/{id}/notes/{noteId} | Удалить Событие Счета поставщику |
| [**deleteInvoiceInPosition**](InvoiceInsApi.md#deleteInvoiceInPosition) | **DELETE** /entity/invoicein/{id}/positions/{positionId} | Удалить позицию Счета поставщику |
| [**deleteInvoiceInPositionsBatch**](InvoiceInsApi.md#deleteInvoiceInPositionsBatch) | **POST** /entity/invoicein/{id}/positions/delete | Массовое удаление позиций Счета поставщику |
| [**getInvoiceInById**](InvoiceInsApi.md#getInvoiceInById) | **GET** /entity/invoicein/{id} | Получить Счет поставщику |
| [**getInvoiceInFile**](InvoiceInsApi.md#getInvoiceInFile) | **GET** /entity/invoicein/{id}/files/{fileId} | Получить файл Счета поставщику |
| [**getInvoiceInFiles**](InvoiceInsApi.md#getInvoiceInFiles) | **GET** /entity/invoicein/{id}/files | Получить файлы Счета поставщику |
| [**getInvoiceInList**](InvoiceInsApi.md#getInvoiceInList) | **GET** /entity/invoicein | Получить список Счетов поставщикам |
| [**getInvoiceInMetadata**](InvoiceInsApi.md#getInvoiceInMetadata) | **GET** /entity/invoicein/metadata | Метаданные Счетов поставщикам |
| [**getInvoiceInMetadataAttribute**](InvoiceInsApi.md#getInvoiceInMetadataAttribute) | **GET** /entity/invoicein/metadata/attributes | Доп. поля InvoiceIn |
| [**getInvoiceInMetadataAttributeById**](InvoiceInsApi.md#getInvoiceInMetadataAttributeById) | **GET** /entity/invoicein/metadata/attributes/{id} | Отдельное доп. поле InvoiceIn |
| [**getInvoiceInMetadataStateById**](InvoiceInsApi.md#getInvoiceInMetadataStateById) | **GET** /entity/invoicein/metadata/states/{id} | Отдельный статус InvoiceIn |
| [**getInvoiceInNoteById**](InvoiceInsApi.md#getInvoiceInNoteById) | **GET** /entity/invoicein/{id}/notes/{noteId} | Получить Событие Счета поставщику по ID |
| [**getInvoiceInNotes**](InvoiceInsApi.md#getInvoiceInNotes) | **GET** /entity/invoicein/{id}/notes | Получить список Событий Счета поставщику |
| [**getInvoiceInPositionById**](InvoiceInsApi.md#getInvoiceInPositionById) | **GET** /entity/invoicein/{id}/positions/{positionId} | Получить позицию Счета поставщику |
| [**getInvoiceInPositions**](InvoiceInsApi.md#getInvoiceInPositions) | **GET** /entity/invoicein/{id}/positions | Получить позиции Счета поставщику |
| [**getInvoiceInTemplate**](InvoiceInsApi.md#getInvoiceInTemplate) | **PUT** /entity/invoicein/new | Шаблон Счета поставщику |
| [**updateInvoiceIn**](InvoiceInsApi.md#updateInvoiceIn) | **PUT** /entity/invoicein/{id} | Изменить Счет поставщику |
| [**updateInvoiceInMetadataAttributeById**](InvoiceInsApi.md#updateInvoiceInMetadataAttributeById) | **PUT** /entity/invoicein/metadata/attributes/{id} | Обновить отдельное доп. поле InvoiceIn |
| [**updateInvoiceInMetadataStateById**](InvoiceInsApi.md#updateInvoiceInMetadataStateById) | **PUT** /entity/invoicein/metadata/states/{id} | Обновить отдельный статус InvoiceIn |
| [**updateInvoiceInNote**](InvoiceInsApi.md#updateInvoiceInNote) | **PUT** /entity/invoicein/{id}/notes/{noteId} | Обновить Событие Счета поставщику |
| [**updateInvoiceInPosition**](InvoiceInsApi.md#updateInvoiceInPosition) | **PUT** /entity/invoicein/{id}/positions/{positionId} | Изменить позицию Счета поставщику |



## addInvoiceInFiles

> List&lt;ModelFile&gt; addInvoiceInFiles(id, fileUpload, accept, acceptEncoding, contentType)

Добавить файлы к Счету поставщику

Добавить новые Файлы к Счету поставщику. В одном запросе можно добавить максимум 10 Файлов. В поле &#x60;content&#x60; нужно указать файл, закодированный в Base64, в поле &#x60;filename&#x60; — имя файла с расширением. 

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.InvoiceInsApi;

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

        InvoiceInsApi apiInstance = new InvoiceInsApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        List<@Valid FileUpload> fileUpload = Arrays.asList(); // List<@Valid FileUpload> | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            List<ModelFile> result = apiInstance.addInvoiceInFiles(id, fileUpload, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvoiceInsApi#addInvoiceInFiles");
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
| **fileUpload** | [**List&lt;@Valid FileUpload&gt;**](FileUpload.md)|  | |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**List&lt;ModelFile&gt;**](ModelFile.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Файлы успешно добавлены. Результат — массив всех Файлов Счета поставщику. |  -  |
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |


## createInvoiceIn

> InvoiceIn createInvoiceIn(invoiceIn, expand, accept, acceptEncoding, contentType)

Создать Счет поставщику

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.InvoiceInsApi;

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

        InvoiceInsApi apiInstance = new InvoiceInsApi(defaultClient);
        InvoiceIn invoiceIn = new InvoiceIn(); // InvoiceIn | 
        String expand = "expand_example"; // String | Замена ссылок объектами с помощью expand
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            InvoiceIn result = apiInstance.createInvoiceIn(invoiceIn, expand, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvoiceInsApi#createInvoiceIn");
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
| **invoiceIn** | [**InvoiceIn**](InvoiceIn.md)|  | |
| **expand** | **String**| Замена ссылок объектами с помощью expand | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**InvoiceIn**](InvoiceIn.md)

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


## createInvoiceInBatch

> List&lt;CreateInvoiceInBatch200ResponseInner&gt; createInvoiceInBatch(invoiceIn, expand, accept, acceptEncoding, contentType)

Массовое создание и обновление Счетов поставщикам

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.InvoiceInsApi;

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

        InvoiceInsApi apiInstance = new InvoiceInsApi(defaultClient);
        List<@Valid InvoiceIn> invoiceIn = Arrays.asList(); // List<@Valid InvoiceIn> | 
        String expand = "expand_example"; // String | Замена ссылок объектами с помощью expand
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            List<CreateInvoiceInBatch200ResponseInner> result = apiInstance.createInvoiceInBatch(invoiceIn, expand, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvoiceInsApi#createInvoiceInBatch");
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
| **invoiceIn** | [**List&lt;@Valid InvoiceIn&gt;**](InvoiceIn.md)|  | |
| **expand** | **String**| Замена ссылок объектами с помощью expand | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**List&lt;CreateInvoiceInBatch200ResponseInner&gt;**](CreateInvoiceInBatch200ResponseInner.md)

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


## createInvoiceInMetadataAttribute

> AttributeMetaInfo createInvoiceInMetadataAttribute(attributeMetaInfo, accept, acceptEncoding, contentType)

Создать Доп. поле InvoiceIn

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.InvoiceInsApi;

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

        InvoiceInsApi apiInstance = new InvoiceInsApi(defaultClient);
        AttributeMetaInfo attributeMetaInfo = new AttributeMetaInfo(); // AttributeMetaInfo | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            AttributeMetaInfo result = apiInstance.createInvoiceInMetadataAttribute(attributeMetaInfo, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvoiceInsApi#createInvoiceInMetadataAttribute");
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


## createInvoiceInNote

> List&lt;EventNote&gt; createInvoiceInNote(id, eventNote, accept, acceptEncoding, contentType)

Добавить Событие Счета поставщику

Запрос на добавление одного События Счета поставщику

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.InvoiceInsApi;

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

        InvoiceInsApi apiInstance = new InvoiceInsApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        EventNote eventNote = new EventNote(); // EventNote | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            List<EventNote> result = apiInstance.createInvoiceInNote(id, eventNote, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvoiceInsApi#createInvoiceInNote");
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
| **eventNote** | [**EventNote**](EventNote.md)|  | |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**List&lt;EventNote&gt;**](EventNote.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Событие успешно создано |  -  |
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |


## createInvoiceInPositions

> InvoiceInPosition createInvoiceInPositions(id, invoiceInPosition, expand, accept, acceptEncoding, contentType)

Создать позицию Счета поставщику

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.InvoiceInsApi;

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

        InvoiceInsApi apiInstance = new InvoiceInsApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        InvoiceInPosition invoiceInPosition = new InvoiceInPosition(); // InvoiceInPosition | 
        String expand = "expand_example"; // String | Замена ссылок объектами с помощью expand
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            InvoiceInPosition result = apiInstance.createInvoiceInPositions(id, invoiceInPosition, expand, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvoiceInsApi#createInvoiceInPositions");
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
| **invoiceInPosition** | [**InvoiceInPosition**](InvoiceInPosition.md)|  | |
| **expand** | **String**| Замена ссылок объектами с помощью expand | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**InvoiceInPosition**](InvoiceInPosition.md)

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


## createInvoiceInPositionsBatch

> List&lt;CreateInvoiceInPositionsBatch200ResponseInner&gt; createInvoiceInPositionsBatch(id, invoiceInPosition, expand, accept, acceptEncoding, contentType)

Создать позиции Счета поставщику

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.InvoiceInsApi;

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

        InvoiceInsApi apiInstance = new InvoiceInsApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        List<@Valid InvoiceInPosition> invoiceInPosition = Arrays.asList(); // List<@Valid InvoiceInPosition> | 
        String expand = "expand_example"; // String | Замена ссылок объектами с помощью expand
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            List<CreateInvoiceInPositionsBatch200ResponseInner> result = apiInstance.createInvoiceInPositionsBatch(id, invoiceInPosition, expand, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvoiceInsApi#createInvoiceInPositionsBatch");
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
| **invoiceInPosition** | [**List&lt;@Valid InvoiceInPosition&gt;**](InvoiceInPosition.md)|  | |
| **expand** | **String**| Замена ссылок объектами с помощью expand | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**List&lt;CreateInvoiceInPositionsBatch200ResponseInner&gt;**](CreateInvoiceInPositionsBatch200ResponseInner.md)

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


## deleteInvoiceIn

> deleteInvoiceIn(id, accept, acceptEncoding, contentType)

Удалить Счет поставщику

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.InvoiceInsApi;

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

        InvoiceInsApi apiInstance = new InvoiceInsApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            apiInstance.deleteInvoiceIn(id, accept, acceptEncoding, contentType);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvoiceInsApi#deleteInvoiceIn");
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
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

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


## deleteInvoiceInBatch

> List&lt;DeleteInvoiceOutBatch200ResponseInner&gt; deleteInvoiceInBatch(invoiceIn, accept, acceptEncoding, contentType)

Массовое удаление Счетов поставщикам

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.InvoiceInsApi;

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

        InvoiceInsApi apiInstance = new InvoiceInsApi(defaultClient);
        List<@Valid InvoiceIn> invoiceIn = Arrays.asList(); // List<@Valid InvoiceIn> | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            List<DeleteInvoiceOutBatch200ResponseInner> result = apiInstance.deleteInvoiceInBatch(invoiceIn, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvoiceInsApi#deleteInvoiceInBatch");
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
| **invoiceIn** | [**List&lt;@Valid InvoiceIn&gt;**](InvoiceIn.md)|  | |
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
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |


## deleteInvoiceInFile

> deleteInvoiceInFile(id, fileId, accept, acceptEncoding)

Удалить файл Счета поставщику

Удаление Файла Счета поставщику.

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.InvoiceInsApi;

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

        InvoiceInsApi apiInstance = new InvoiceInsApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        UUID fileId = UUID.randomUUID(); // UUID | ID файла
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            apiInstance.deleteInvoiceInFile(id, fileId, accept, acceptEncoding);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvoiceInsApi#deleteInvoiceInFile");
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
| **fileId** | **UUID**| ID файла | |
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
| **200** | Файл успешно удалён |  -  |
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |


## deleteInvoiceInMetadataAttributeById

> deleteInvoiceInMetadataAttributeById(id, accept, acceptEncoding, contentType)

Удалить отдельное доп. поле InvoiceIn

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.InvoiceInsApi;

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

        InvoiceInsApi apiInstance = new InvoiceInsApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            apiInstance.deleteInvoiceInMetadataAttributeById(id, accept, acceptEncoding, contentType);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvoiceInsApi#deleteInvoiceInMetadataAttributeById");
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
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

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


## deleteInvoiceInMetadataStateById

> deleteInvoiceInMetadataStateById(id, accept, acceptEncoding, contentType)

Удалить отдельный статус InvoiceIn

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.InvoiceInsApi;

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

        InvoiceInsApi apiInstance = new InvoiceInsApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            apiInstance.deleteInvoiceInMetadataStateById(id, accept, acceptEncoding, contentType);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvoiceInsApi#deleteInvoiceInMetadataStateById");
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
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

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


## deleteInvoiceInNote

> deleteInvoiceInNote(id, noteId, accept, acceptEncoding)

Удалить Событие Счета поставщику

Запрос на удаление одного События Счета поставщику

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.InvoiceInsApi;

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

        InvoiceInsApi apiInstance = new InvoiceInsApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        UUID noteId = UUID.randomUUID(); // UUID | ID События
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            apiInstance.deleteInvoiceInNote(id, noteId, accept, acceptEncoding);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvoiceInsApi#deleteInvoiceInNote");
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
| **noteId** | **UUID**| ID События | |
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
| **204** | Событие успешно удалено |  -  |
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |


## deleteInvoiceInPosition

> deleteInvoiceInPosition(id, positionId, expand, accept, acceptEncoding, contentType)

Удалить позицию Счета поставщику

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.InvoiceInsApi;

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

        InvoiceInsApi apiInstance = new InvoiceInsApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        UUID positionId = UUID.randomUUID(); // UUID | ID позиции
        String expand = "expand_example"; // String | Замена ссылок объектами с помощью expand
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            apiInstance.deleteInvoiceInPosition(id, positionId, expand, accept, acceptEncoding, contentType);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvoiceInsApi#deleteInvoiceInPosition");
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
| **positionId** | **UUID**| ID позиции | |
| **expand** | **String**| Замена ссылок объектами с помощью expand | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

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


## deleteInvoiceInPositionsBatch

> List&lt;DeleteInvoiceOutBatch200ResponseInner&gt; deleteInvoiceInPositionsBatch(id, invoiceInPosition, accept, acceptEncoding, contentType)

Массовое удаление позиций Счета поставщику

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.InvoiceInsApi;

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

        InvoiceInsApi apiInstance = new InvoiceInsApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        List<@Valid InvoiceInPosition> invoiceInPosition = Arrays.asList(); // List<@Valid InvoiceInPosition> | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            List<DeleteInvoiceOutBatch200ResponseInner> result = apiInstance.deleteInvoiceInPositionsBatch(id, invoiceInPosition, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvoiceInsApi#deleteInvoiceInPositionsBatch");
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
| **invoiceInPosition** | [**List&lt;@Valid InvoiceInPosition&gt;**](InvoiceInPosition.md)|  | |
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
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |


## getInvoiceInById

> InvoiceIn getInvoiceInById(id, expand, fields, accept, acceptEncoding)

Получить Счет поставщику

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.InvoiceInsApi;

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

        InvoiceInsApi apiInstance = new InvoiceInsApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        String expand = "expand_example"; // String | Замена ссылок объектами с помощью expand
        String fields = "minimumStock"; // String | Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - `minimumStock` — неснижаемый остаток (товар, модификация) - `downloadPermanentHref` — постоянная ссылка на изображение (платный тариф) - `stock` — остатки и себестоимость в позициях документов - `declaration` — прослеживаемость импортных товаров в позициях документов 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            InvoiceIn result = apiInstance.getInvoiceInById(id, expand, fields, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvoiceInsApi#getInvoiceInById");
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
| **fields** | **String**| Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - &#x60;minimumStock&#x60; — неснижаемый остаток (товар, модификация) - &#x60;downloadPermanentHref&#x60; — постоянная ссылка на изображение (платный тариф) - &#x60;stock&#x60; — остатки и себестоимость в позициях документов - &#x60;declaration&#x60; — прослеживаемость импортных товаров в позициях документов  | [optional] [enum: minimumStock, downloadPermanentHref, stock, declaration] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |

### Return type

[**InvoiceIn**](InvoiceIn.md)

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


## getInvoiceInFile

> ModelFile getInvoiceInFile(id, fileId, accept, acceptEncoding)

Получить файл Счета поставщику

Получение Файла Счета поставщику.

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.InvoiceInsApi;

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

        InvoiceInsApi apiInstance = new InvoiceInsApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        UUID fileId = UUID.randomUUID(); // UUID | ID файла
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            ModelFile result = apiInstance.getInvoiceInFile(id, fileId, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvoiceInsApi#getInvoiceInFile");
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
| **fileId** | **UUID**| ID файла | |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |

### Return type

[**ModelFile**](ModelFile.md)

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


## getInvoiceInFiles

> GetProductFiles200Response getInvoiceInFiles(id, limit, offset, accept, acceptEncoding)

Получить файлы Счета поставщику

Запрос на получение списка всех Файлов данного Счета поставщику.

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.InvoiceInsApi;

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

        InvoiceInsApi apiInstance = new InvoiceInsApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        Integer limit = 1000; // Integer | Максимальное количество элементов в выданном списке (максимум 1000)
        Integer offset = 0; // Integer | Отступ в выданном списке
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            GetProductFiles200Response result = apiInstance.getInvoiceInFiles(id, limit, offset, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvoiceInsApi#getInvoiceInFiles");
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
| **limit** | **Integer**| Максимальное количество элементов в выданном списке (максимум 1000) | [optional] [default to 1000] |
| **offset** | **Integer**| Отступ в выданном списке | [optional] [default to 0] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |

### Return type

[**GetProductFiles200Response**](GetProductFiles200Response.md)

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


## getInvoiceInList

> InvoiceInList getInvoiceInList(limit, offset, search, expand, fields, accept, acceptEncoding)

Получить список Счетов поставщикам

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.InvoiceInsApi;

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

        InvoiceInsApi apiInstance = new InvoiceInsApi(defaultClient);
        Integer limit = 1000; // Integer | Максимальное количество элементов в выданном списке (максимум 1000)
        Integer offset = 0; // Integer | Отступ в выданном списке
        String search = "search_example"; // String | Контекстный поиск по строковым полям сущностей
        String expand = "expand_example"; // String | Замена ссылок объектами с помощью expand
        String fields = "minimumStock"; // String | Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - `minimumStock` — неснижаемый остаток (товар, модификация) - `downloadPermanentHref` — постоянная ссылка на изображение (платный тариф) - `stock` — остатки и себестоимость в позициях документов - `declaration` — прослеживаемость импортных товаров в позициях документов 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            InvoiceInList result = apiInstance.getInvoiceInList(limit, offset, search, expand, fields, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvoiceInsApi#getInvoiceInList");
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
| **expand** | **String**| Замена ссылок объектами с помощью expand | [optional] |
| **fields** | **String**| Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - &#x60;minimumStock&#x60; — неснижаемый остаток (товар, модификация) - &#x60;downloadPermanentHref&#x60; — постоянная ссылка на изображение (платный тариф) - &#x60;stock&#x60; — остатки и себестоимость в позициях документов - &#x60;declaration&#x60; — прослеживаемость импортных товаров в позициях документов  | [optional] [enum: minimumStock, downloadPermanentHref, stock, declaration] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |

### Return type

[**InvoiceInList**](InvoiceInList.md)

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


## getInvoiceInMetadata

> DocumentMetadata getInvoiceInMetadata(accept, acceptEncoding, contentType)

Метаданные Счетов поставщикам

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.InvoiceInsApi;

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

        InvoiceInsApi apiInstance = new InvoiceInsApi(defaultClient);
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            DocumentMetadata result = apiInstance.getInvoiceInMetadata(accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvoiceInsApi#getInvoiceInMetadata");
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
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

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


## getInvoiceInMetadataAttribute

> AttributeMetaInfoList getInvoiceInMetadataAttribute(offset, limit, accept, acceptEncoding, contentType)

Доп. поля InvoiceIn

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.InvoiceInsApi;

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

        InvoiceInsApi apiInstance = new InvoiceInsApi(defaultClient);
        Integer offset = 0; // Integer | Отступ в выданном списке
        Integer limit = 1000; // Integer | Максимальное количество элементов в выданном списке (максимум 1000)
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            AttributeMetaInfoList result = apiInstance.getInvoiceInMetadataAttribute(offset, limit, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvoiceInsApi#getInvoiceInMetadataAttribute");
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
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

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


## getInvoiceInMetadataAttributeById

> AttributeMetaInfo getInvoiceInMetadataAttributeById(id, accept, acceptEncoding, contentType)

Отдельное доп. поле InvoiceIn

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.InvoiceInsApi;

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

        InvoiceInsApi apiInstance = new InvoiceInsApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            AttributeMetaInfo result = apiInstance.getInvoiceInMetadataAttributeById(id, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvoiceInsApi#getInvoiceInMetadataAttributeById");
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
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

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


## getInvoiceInMetadataStateById

> State getInvoiceInMetadataStateById(id, accept, acceptEncoding, contentType)

Отдельный статус InvoiceIn

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.InvoiceInsApi;

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

        InvoiceInsApi apiInstance = new InvoiceInsApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            State result = apiInstance.getInvoiceInMetadataStateById(id, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvoiceInsApi#getInvoiceInMetadataStateById");
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
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

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


## getInvoiceInNoteById

> EventNote getInvoiceInNoteById(id, noteId, accept, acceptEncoding)

Получить Событие Счета поставщику по ID

Запрос на получение одного События Счета поставщику

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.InvoiceInsApi;

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

        InvoiceInsApi apiInstance = new InvoiceInsApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        UUID noteId = UUID.randomUUID(); // UUID | ID События
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            EventNote result = apiInstance.getInvoiceInNoteById(id, noteId, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvoiceInsApi#getInvoiceInNoteById");
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
| **noteId** | **UUID**| ID События | |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |

### Return type

[**EventNote**](EventNote.md)

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


## getInvoiceInNotes

> EventNoteList getInvoiceInNotes(id, limit, offset, expand, accept, acceptEncoding)

Получить список Событий Счета поставщику

Запрос на получение всех Событий Счета поставщику для данной учетной записи

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.InvoiceInsApi;

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

        InvoiceInsApi apiInstance = new InvoiceInsApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        Integer limit = 1000; // Integer | Максимальное количество элементов в выданном списке (максимум 1000)
        Integer offset = 0; // Integer | Отступ в выданном списке
        String expand = "expand_example"; // String | Замена ссылок объектами с помощью expand
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            EventNoteList result = apiInstance.getInvoiceInNotes(id, limit, offset, expand, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvoiceInsApi#getInvoiceInNotes");
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
| **limit** | **Integer**| Максимальное количество элементов в выданном списке (максимум 1000) | [optional] [default to 1000] |
| **offset** | **Integer**| Отступ в выданном списке | [optional] [default to 0] |
| **expand** | **String**| Замена ссылок объектами с помощью expand | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |

### Return type

[**EventNoteList**](EventNoteList.md)

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


## getInvoiceInPositionById

> InvoiceInPosition getInvoiceInPositionById(id, positionId, expand, fields, accept, acceptEncoding, contentType)

Получить позицию Счета поставщику

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.InvoiceInsApi;

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

        InvoiceInsApi apiInstance = new InvoiceInsApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        UUID positionId = UUID.randomUUID(); // UUID | ID позиции
        String expand = "expand_example"; // String | Замена ссылок объектами с помощью expand
        String fields = "minimumStock"; // String | Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - `minimumStock` — неснижаемый остаток (товар, модификация) - `downloadPermanentHref` — постоянная ссылка на изображение (платный тариф) - `stock` — остатки и себестоимость в позициях документов - `declaration` — прослеживаемость импортных товаров в позициях документов 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            InvoiceInPosition result = apiInstance.getInvoiceInPositionById(id, positionId, expand, fields, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvoiceInsApi#getInvoiceInPositionById");
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
| **positionId** | **UUID**| ID позиции | |
| **expand** | **String**| Замена ссылок объектами с помощью expand | [optional] |
| **fields** | **String**| Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - &#x60;minimumStock&#x60; — неснижаемый остаток (товар, модификация) - &#x60;downloadPermanentHref&#x60; — постоянная ссылка на изображение (платный тариф) - &#x60;stock&#x60; — остатки и себестоимость в позициях документов - &#x60;declaration&#x60; — прослеживаемость импортных товаров в позициях документов  | [optional] [enum: minimumStock, downloadPermanentHref, stock, declaration] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**InvoiceInPosition**](InvoiceInPosition.md)

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


## getInvoiceInPositions

> InvoiceInPositionList getInvoiceInPositions(id, limit, offset, expand, fields, accept, acceptEncoding, contentType)

Получить позиции Счета поставщику

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.InvoiceInsApi;

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

        InvoiceInsApi apiInstance = new InvoiceInsApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        Integer limit = 1000; // Integer | Максимальное количество элементов в выданном списке (максимум 1000)
        Integer offset = 0; // Integer | Отступ в выданном списке
        String expand = "expand_example"; // String | Замена ссылок объектами с помощью expand
        String fields = "minimumStock"; // String | Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - `minimumStock` — неснижаемый остаток (товар, модификация) - `downloadPermanentHref` — постоянная ссылка на изображение (платный тариф) - `stock` — остатки и себестоимость в позициях документов - `declaration` — прослеживаемость импортных товаров в позициях документов 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            InvoiceInPositionList result = apiInstance.getInvoiceInPositions(id, limit, offset, expand, fields, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvoiceInsApi#getInvoiceInPositions");
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
| **limit** | **Integer**| Максимальное количество элементов в выданном списке (максимум 1000) | [optional] [default to 1000] |
| **offset** | **Integer**| Отступ в выданном списке | [optional] [default to 0] |
| **expand** | **String**| Замена ссылок объектами с помощью expand | [optional] |
| **fields** | **String**| Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - &#x60;minimumStock&#x60; — неснижаемый остаток (товар, модификация) - &#x60;downloadPermanentHref&#x60; — постоянная ссылка на изображение (платный тариф) - &#x60;stock&#x60; — остатки и себестоимость в позициях документов - &#x60;declaration&#x60; — прослеживаемость импортных товаров в позициях документов  | [optional] [enum: minimumStock, downloadPermanentHref, stock, declaration] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**InvoiceInPositionList**](InvoiceInPositionList.md)

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


## getInvoiceInTemplate

> InvoiceIn getInvoiceInTemplate(accept, acceptEncoding, contentType, body)

Шаблон Счета поставщику

Предзаполненный шаблон Счета поставщику. Пустое тело — стандартные значения без привязки к документу; в теле можно передать, например, &#x60;purchaseOrder&#x60; или &#x60;supplies&#x60; для шаблона на основе документа. 

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.InvoiceInsApi;

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

        InvoiceInsApi apiInstance = new InvoiceInsApi(defaultClient);
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        Object body = null; // Object | 
        try {
            InvoiceIn result = apiInstance.getInvoiceInTemplate(accept, acceptEncoding, contentType, body);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvoiceInsApi#getInvoiceInTemplate");
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
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |
| **body** | **Object**|  | [optional] |

### Return type

[**InvoiceIn**](InvoiceIn.md)

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


## updateInvoiceIn

> InvoiceIn updateInvoiceIn(id, invoiceIn, expand, fields, accept, acceptEncoding, contentType)

Изменить Счет поставщику

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.InvoiceInsApi;

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

        InvoiceInsApi apiInstance = new InvoiceInsApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        InvoiceIn invoiceIn = new InvoiceIn(); // InvoiceIn | 
        String expand = "expand_example"; // String | Замена ссылок объектами с помощью expand
        String fields = "minimumStock"; // String | Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - `minimumStock` — неснижаемый остаток (товар, модификация) - `downloadPermanentHref` — постоянная ссылка на изображение (платный тариф) - `stock` — остатки и себестоимость в позициях документов - `declaration` — прослеживаемость импортных товаров в позициях документов 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            InvoiceIn result = apiInstance.updateInvoiceIn(id, invoiceIn, expand, fields, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvoiceInsApi#updateInvoiceIn");
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
| **invoiceIn** | [**InvoiceIn**](InvoiceIn.md)|  | |
| **expand** | **String**| Замена ссылок объектами с помощью expand | [optional] |
| **fields** | **String**| Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - &#x60;minimumStock&#x60; — неснижаемый остаток (товар, модификация) - &#x60;downloadPermanentHref&#x60; — постоянная ссылка на изображение (платный тариф) - &#x60;stock&#x60; — остатки и себестоимость в позициях документов - &#x60;declaration&#x60; — прослеживаемость импортных товаров в позициях документов  | [optional] [enum: minimumStock, downloadPermanentHref, stock, declaration] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**InvoiceIn**](InvoiceIn.md)

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


## updateInvoiceInMetadataAttributeById

> AttributeMetaInfo updateInvoiceInMetadataAttributeById(id, attributeMetaInfo, accept, acceptEncoding, contentType)

Обновить отдельное доп. поле InvoiceIn

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.InvoiceInsApi;

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

        InvoiceInsApi apiInstance = new InvoiceInsApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        AttributeMetaInfo attributeMetaInfo = new AttributeMetaInfo(); // AttributeMetaInfo | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            AttributeMetaInfo result = apiInstance.updateInvoiceInMetadataAttributeById(id, attributeMetaInfo, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvoiceInsApi#updateInvoiceInMetadataAttributeById");
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


## updateInvoiceInMetadataStateById

> State updateInvoiceInMetadataStateById(id, state, accept, acceptEncoding, contentType)

Обновить отдельный статус InvoiceIn

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.InvoiceInsApi;

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

        InvoiceInsApi apiInstance = new InvoiceInsApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        State state = new State(); // State | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            State result = apiInstance.updateInvoiceInMetadataStateById(id, state, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvoiceInsApi#updateInvoiceInMetadataStateById");
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


## updateInvoiceInNote

> EventNote updateInvoiceInNote(id, noteId, eventNote, accept, acceptEncoding, contentType)

Обновить Событие Счета поставщику

Запрос на обновление одного События Счета поставщику

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.InvoiceInsApi;

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

        InvoiceInsApi apiInstance = new InvoiceInsApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        UUID noteId = UUID.randomUUID(); // UUID | ID События
        EventNote eventNote = new EventNote(); // EventNote | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            EventNote result = apiInstance.updateInvoiceInNote(id, noteId, eventNote, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvoiceInsApi#updateInvoiceInNote");
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
| **noteId** | **UUID**| ID События | |
| **eventNote** | [**EventNote**](EventNote.md)|  | |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**EventNote**](EventNote.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Событие успешно обновлено |  -  |
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |


## updateInvoiceInPosition

> InvoiceInPosition updateInvoiceInPosition(id, positionId, invoiceInPosition, expand, fields, accept, acceptEncoding, contentType)

Изменить позицию Счета поставщику

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.InvoiceInsApi;

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

        InvoiceInsApi apiInstance = new InvoiceInsApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        UUID positionId = UUID.randomUUID(); // UUID | ID позиции
        InvoiceInPosition invoiceInPosition = new InvoiceInPosition(); // InvoiceInPosition | 
        String expand = "expand_example"; // String | Замена ссылок объектами с помощью expand
        String fields = "minimumStock"; // String | Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - `minimumStock` — неснижаемый остаток (товар, модификация) - `downloadPermanentHref` — постоянная ссылка на изображение (платный тариф) - `stock` — остатки и себестоимость в позициях документов - `declaration` — прослеживаемость импортных товаров в позициях документов 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            InvoiceInPosition result = apiInstance.updateInvoiceInPosition(id, positionId, invoiceInPosition, expand, fields, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvoiceInsApi#updateInvoiceInPosition");
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
| **positionId** | **UUID**| ID позиции | |
| **invoiceInPosition** | [**InvoiceInPosition**](InvoiceInPosition.md)|  | |
| **expand** | **String**| Замена ссылок объектами с помощью expand | [optional] |
| **fields** | **String**| Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - &#x60;minimumStock&#x60; — неснижаемый остаток (товар, модификация) - &#x60;downloadPermanentHref&#x60; — постоянная ссылка на изображение (платный тариф) - &#x60;stock&#x60; — остатки и себестоимость в позициях документов - &#x60;declaration&#x60; — прослеживаемость импортных товаров в позициях документов  | [optional] [enum: minimumStock, downloadPermanentHref, stock, declaration] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**InvoiceInPosition**](InvoiceInPosition.md)

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

