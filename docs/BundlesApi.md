# BundlesApi

All URIs are relative to *https://api.moysklad.ru/api/remap/1.2*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**addBundleFile**](BundlesApi.md#addBundleFile) | **POST** /entity/bundle/{id}/files | Добавить файл к Комплекту |
| [**addBundleFiles**](BundlesApi.md#addBundleFiles) | **POST** /entity/bundle/{id}/files/batch | Добавить файлы к Комплекту |
| [**addBundleImage**](BundlesApi.md#addBundleImage) | **POST** /entity/bundle/{id}/images | Добавить изображение к Комплекту |
| [**addBundleImages**](BundlesApi.md#addBundleImages) | **POST** /entity/bundle/{id}/images/batch | Изменить список изображений Комплекта |
| [**createBundle**](BundlesApi.md#createBundle) | **POST** /entity/bundle | Создать Комплект |
| [**createBundleComponent**](BundlesApi.md#createBundleComponent) | **POST** /entity/bundle/{id}/components | Добавить компонент Комплекта |
| [**createBundleComponents**](BundlesApi.md#createBundleComponents) | **POST** /entity/bundle/{id}/components/batch | Массовое добавление и обновление компонентов Комплекта |
| [**createBundlesBatch**](BundlesApi.md#createBundlesBatch) | **POST** /entity/bundle/batch | Массовое создание и обновление Комплектов |
| [**deleteBundle**](BundlesApi.md#deleteBundle) | **DELETE** /entity/bundle/{id} | Удалить Комплект |
| [**deleteBundleComponent**](BundlesApi.md#deleteBundleComponent) | **DELETE** /entity/bundle/{id}/components/{componentId} | Удалить компонент |
| [**deleteBundleComponentsBatch**](BundlesApi.md#deleteBundleComponentsBatch) | **POST** /entity/bundle/{id}/components/delete | Массовое удаление компонентов Комплекта |
| [**deleteBundleFile**](BundlesApi.md#deleteBundleFile) | **DELETE** /entity/bundle/{id}/files/{fileId} | Удалить файл Комплекта |
| [**deleteBundleImage**](BundlesApi.md#deleteBundleImage) | **DELETE** /entity/bundle/{id}/images/{imageId} | Удалить изображение Комплекта |
| [**deleteBundleImages**](BundlesApi.md#deleteBundleImages) | **POST** /entity/bundle/{id}/images/delete | Массовое удаление изображений Комплекта |
| [**deleteBundlesBatch**](BundlesApi.md#deleteBundlesBatch) | **POST** /entity/bundle/delete | Массовое удаление Комплектов |
| [**getBundleById**](BundlesApi.md#getBundleById) | **GET** /entity/bundle/{id} | Получить Комплект |
| [**getBundleComponentById**](BundlesApi.md#getBundleComponentById) | **GET** /entity/bundle/{id}/components/{componentId} | Получить компонент |
| [**getBundleComponents**](BundlesApi.md#getBundleComponents) | **GET** /entity/bundle/{id}/components | Получить компоненты Комплекта |
| [**getBundleFiles**](BundlesApi.md#getBundleFiles) | **GET** /entity/bundle/{id}/files | Получить файлы Комплекта |
| [**getBundleImages**](BundlesApi.md#getBundleImages) | **GET** /entity/bundle/{id}/images | Получить изображения Комплекта |
| [**getBundles**](BundlesApi.md#getBundles) | **GET** /entity/bundle | Получить список комплектов |
| [**updateBundle**](BundlesApi.md#updateBundle) | **PUT** /entity/bundle/{id} | Изменить Комплект |
| [**updateBundleComponent**](BundlesApi.md#updateBundleComponent) | **PUT** /entity/bundle/{id}/components/{componentId} | Изменить компонент |



## addBundleFile

> List&lt;ModelFile&gt; addBundleFile(id, fileUpload, accept, acceptEncoding, contentType)

Добавить файл к Комплекту

Добавить новый Файл к Комплекту. В поле &#x60;content&#x60; нужно указать файл, закодированный в Base64, в поле &#x60;filename&#x60; — имя файла с расширением. 

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.BundlesApi;

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

        BundlesApi apiInstance = new BundlesApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        FileUpload fileUpload = new FileUpload(); // FileUpload | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip"; // String | 
        String contentType = "application/json"; // String | 
        try {
            List<ModelFile> result = apiInstance.addBundleFile(id, fileUpload, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling BundlesApi#addBundleFile");
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
| **fileUpload** | [**FileUpload**](FileUpload.md)|  | |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**List&lt;ModelFile&gt;**](ModelFile.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Файл успешно добавлен. Результат — массив всех Файлов Комплекта. |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## addBundleFiles

> List&lt;ModelFile&gt; addBundleFiles(id, fileUpload, accept, acceptEncoding, contentType)

Добавить файлы к Комплекту

Добавить новые Файлы к Комплекту. В одном запросе можно добавить максимум 10 Файлов. В поле &#x60;content&#x60; нужно указать файл, закодированный в Base64, в поле &#x60;filename&#x60; — имя файла с расширением. 

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.BundlesApi;

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

        BundlesApi apiInstance = new BundlesApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        List<FileUpload> fileUpload = Arrays.asList(); // List<FileUpload> | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip"; // String | 
        String contentType = "application/json"; // String | 
        try {
            List<ModelFile> result = apiInstance.addBundleFiles(id, fileUpload, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling BundlesApi#addBundleFiles");
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
| **fileUpload** | [**List&lt;FileUpload&gt;**](FileUpload.md)|  | |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**List&lt;ModelFile&gt;**](ModelFile.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Файлы успешно добавлены. Результат — массив всех Файлов Комплекта. |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## addBundleImage

> List&lt;Image&gt; addBundleImage(id, fileUpload, accept, acceptEncoding, contentType)

Добавить изображение к Комплекту

Добавить новое Изображение к Комплекту. В поле &#x60;content&#x60; нужно указать изображение, закодированное в Base64, в поле &#x60;filename&#x60; — имя файла с расширением. У Комплекта может быть не более 10 Изображений. 

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.BundlesApi;

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

        BundlesApi apiInstance = new BundlesApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        FileUpload fileUpload = new FileUpload(); // FileUpload | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip"; // String | 
        String contentType = "application/json"; // String | 
        try {
            List<Image> result = apiInstance.addBundleImage(id, fileUpload, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling BundlesApi#addBundleImage");
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
| **fileUpload** | [**FileUpload**](FileUpload.md)|  | |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**List&lt;Image&gt;**](Image.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Изображение успешно добавлено. Результат — массив всех Изображений Комплекта. |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## addBundleImages

> List&lt;Image&gt; addBundleImages(id, fileUpload, accept, acceptEncoding, contentType)

Изменить список изображений Комплекта

Установить список Изображений Комплекта. В теле запроса нужно передать массив Изображений, которые должны быть у Комплекта. Чтобы оставить существующие Изображения, передайте их метаданные. Для новых Изображений в поле &#x60;content&#x60; нужно указать изображение, закодированное в Base64, в поле &#x60;filename&#x60; — имя файла с расширением. У Комплекта может быть не более 10 Изображений. 

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.BundlesApi;

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

        BundlesApi apiInstance = new BundlesApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        List<FileUpload> fileUpload = Arrays.asList(); // List<FileUpload> | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip"; // String | 
        String contentType = "application/json"; // String | 
        try {
            List<Image> result = apiInstance.addBundleImages(id, fileUpload, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling BundlesApi#addBundleImages");
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
| **fileUpload** | [**List&lt;FileUpload&gt;**](FileUpload.md)|  | |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**List&lt;Image&gt;**](Image.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Список Изображений успешно изменен. Результат — массив всех Изображений Комплекта. |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## createBundle

> Bundle createBundle(bundle, accept, acceptEncoding, expand, contentType)

Создать Комплект

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.BundlesApi;

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

        BundlesApi apiInstance = new BundlesApi(defaultClient);
        Bundle bundle = new Bundle(); // Bundle | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip"; // String | 
        String expand = "expand_example"; // String | Замена ссылок объектами с помощью expand
        String contentType = "application/json"; // String | 
        try {
            Bundle result = apiInstance.createBundle(bundle, accept, acceptEncoding, expand, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling BundlesApi#createBundle");
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
| **bundle** | [**Bundle**](Bundle.md)|  | |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip] |
| **expand** | **String**| Замена ссылок объектами с помощью expand | [optional] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**Bundle**](Bundle.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## createBundleComponent

> BundleComponent createBundleComponent(id, bundleComponent, accept, acceptEncoding, expand, contentType)

Добавить компонент Комплекта

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.BundlesApi;

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

        BundlesApi apiInstance = new BundlesApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        BundleComponent bundleComponent = new BundleComponent(); // BundleComponent | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip"; // String | 
        String expand = "expand_example"; // String | Замена ссылок объектами с помощью expand
        String contentType = "application/json"; // String | 
        try {
            BundleComponent result = apiInstance.createBundleComponent(id, bundleComponent, accept, acceptEncoding, expand, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling BundlesApi#createBundleComponent");
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
| **bundleComponent** | [**BundleComponent**](BundleComponent.md)|  | |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip] |
| **expand** | **String**| Замена ссылок объектами с помощью expand | [optional] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**BundleComponent**](BundleComponent.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## createBundleComponents

> List&lt;BatchResponseEntity&gt; createBundleComponents(id, bundleComponent, accept, acceptEncoding, expand, contentType)

Массовое добавление и обновление компонентов Комплекта

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.BundlesApi;

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

        BundlesApi apiInstance = new BundlesApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        List<BundleComponent> bundleComponent = Arrays.asList(); // List<BundleComponent> | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip"; // String | 
        String expand = "expand_example"; // String | Замена ссылок объектами с помощью expand
        String contentType = "application/json"; // String | 
        try {
            List<BatchResponseEntity> result = apiInstance.createBundleComponents(id, bundleComponent, accept, acceptEncoding, expand, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling BundlesApi#createBundleComponents");
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
| **bundleComponent** | [**List&lt;BundleComponent&gt;**](BundleComponent.md)|  | |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip] |
| **expand** | **String**| Замена ссылок объектами с помощью expand | [optional] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**List&lt;BatchResponseEntity&gt;**](BatchResponseEntity.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос |  -  |
| **404** | Ошибка массовой операции: объект errors или массив результатов по каждому элементу  |  -  |
| **412** | Ошибка массовой операции: объект errors или массив результатов по каждому элементу  |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## createBundlesBatch

> List&lt;BatchResponseEntity&gt; createBundlesBatch(bundle, accept, acceptEncoding, expand, contentType)

Массовое создание и обновление Комплектов

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.BundlesApi;

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

        BundlesApi apiInstance = new BundlesApi(defaultClient);
        List<Bundle> bundle = Arrays.asList(); // List<Bundle> | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip"; // String | 
        String expand = "expand_example"; // String | Замена ссылок объектами с помощью expand
        String contentType = "application/json"; // String | 
        try {
            List<BatchResponseEntity> result = apiInstance.createBundlesBatch(bundle, accept, acceptEncoding, expand, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling BundlesApi#createBundlesBatch");
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
| **bundle** | [**List&lt;Bundle&gt;**](Bundle.md)|  | |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip] |
| **expand** | **String**| Замена ссылок объектами с помощью expand | [optional] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**List&lt;BatchResponseEntity&gt;**](BatchResponseEntity.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос |  -  |
| **404** | Ошибка массовой операции: объект errors или массив результатов по каждому элементу  |  -  |
| **412** | Ошибка массовой операции: объект errors или массив результатов по каждому элементу  |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## deleteBundle

> deleteBundle(id, accept, acceptEncoding)

Удалить Комплект

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.BundlesApi;

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

        BundlesApi apiInstance = new BundlesApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip"; // String | 
        try {
            apiInstance.deleteBundle(id, accept, acceptEncoding);
        } catch (ApiException e) {
            System.err.println("Exception when calling BundlesApi#deleteBundle");
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
| **acceptEncoding** | **String**|  | [optional] [default to gzip] |

### Return type

null (empty response body)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## deleteBundleComponent

> deleteBundleComponent(id, componentId, accept, acceptEncoding)

Удалить компонент

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.BundlesApi;

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

        BundlesApi apiInstance = new BundlesApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        UUID componentId = UUID.randomUUID(); // UUID | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip"; // String | 
        try {
            apiInstance.deleteBundleComponent(id, componentId, accept, acceptEncoding);
        } catch (ApiException e) {
            System.err.println("Exception when calling BundlesApi#deleteBundleComponent");
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
| **componentId** | **UUID**|  | |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip] |

### Return type

null (empty response body)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## deleteBundleComponentsBatch

> List&lt;DeleteRowResult&gt; deleteBundleComponentsBatch(id, bundleComponent, accept, acceptEncoding, contentType)

Массовое удаление компонентов Комплекта

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.BundlesApi;

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

        BundlesApi apiInstance = new BundlesApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        List<BundleComponent> bundleComponent = Arrays.asList(); // List<BundleComponent> | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip"; // String | 
        String contentType = "application/json"; // String | 
        try {
            List<DeleteRowResult> result = apiInstance.deleteBundleComponentsBatch(id, bundleComponent, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling BundlesApi#deleteBundleComponentsBatch");
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
| **bundleComponent** | [**List&lt;BundleComponent&gt;**](BundleComponent.md)|  | |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**List&lt;DeleteRowResult&gt;**](DeleteRowResult.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Результат по каждому элементу (успех или объект ошибки) |  -  |
| **404** | Ошибка массовой операции: объект errors или массив результатов по каждому элементу  |  -  |
| **412** | Ошибка массовой операции: объект errors или массив результатов по каждому элементу  |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## deleteBundleFile

> deleteBundleFile(id, fileId, accept, acceptEncoding)

Удалить файл Комплекта

Удаление Файла Комплекта.

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.BundlesApi;

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

        BundlesApi apiInstance = new BundlesApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        UUID fileId = UUID.randomUUID(); // UUID | ID файла
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip"; // String | 
        try {
            apiInstance.deleteBundleFile(id, fileId, accept, acceptEncoding);
        } catch (ApiException e) {
            System.err.println("Exception when calling BundlesApi#deleteBundleFile");
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
| **acceptEncoding** | **String**|  | [optional] [default to gzip] |

### Return type

null (empty response body)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Файл успешно удалён |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## deleteBundleImage

> deleteBundleImage(id, imageId, accept, acceptEncoding)

Удалить изображение Комплекта

Удаление Изображения Комплекта.

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.BundlesApi;

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

        BundlesApi apiInstance = new BundlesApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        UUID imageId = UUID.randomUUID(); // UUID | ID изображения
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip"; // String | 
        try {
            apiInstance.deleteBundleImage(id, imageId, accept, acceptEncoding);
        } catch (ApiException e) {
            System.err.println("Exception when calling BundlesApi#deleteBundleImage");
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
| **imageId** | **UUID**| ID изображения | |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip] |

### Return type

null (empty response body)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Изображение успешно удалено |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## deleteBundleImages

> deleteBundleImages(id, deleteProductImagesRequestInner, accept, acceptEncoding, contentType)

Массовое удаление изображений Комплекта

Массовое удаление Изображений Комплекта.

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.BundlesApi;

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

        BundlesApi apiInstance = new BundlesApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        List<DeleteProductImagesRequestInner> deleteProductImagesRequestInner = Arrays.asList(); // List<DeleteProductImagesRequestInner> | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip"; // String | 
        String contentType = "application/json"; // String | 
        try {
            apiInstance.deleteBundleImages(id, deleteProductImagesRequestInner, accept, acceptEncoding, contentType);
        } catch (ApiException e) {
            System.err.println("Exception when calling BundlesApi#deleteBundleImages");
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
| **deleteProductImagesRequestInner** | [**List&lt;DeleteProductImagesRequestInner&gt;**](DeleteProductImagesRequestInner.md)|  | |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

null (empty response body)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Изображения успешно удалены |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## deleteBundlesBatch

> List&lt;DeleteRowResult&gt; deleteBundlesBatch(bundle, accept, acceptEncoding, contentType)

Массовое удаление Комплектов

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.BundlesApi;

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

        BundlesApi apiInstance = new BundlesApi(defaultClient);
        List<Bundle> bundle = Arrays.asList(); // List<Bundle> | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip"; // String | 
        String contentType = "application/json"; // String | 
        try {
            List<DeleteRowResult> result = apiInstance.deleteBundlesBatch(bundle, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling BundlesApi#deleteBundlesBatch");
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
| **bundle** | [**List&lt;Bundle&gt;**](Bundle.md)|  | |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**List&lt;DeleteRowResult&gt;**](DeleteRowResult.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос |  -  |
| **404** | Ошибка массовой операции: объект errors или массив результатов по каждому элементу  |  -  |
| **412** | Ошибка массовой операции: объект errors или массив результатов по каждому элементу  |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## getBundleById

> Bundle getBundleById(id, expand, accept, acceptEncoding)

Получить Комплект

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.BundlesApi;

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

        BundlesApi apiInstance = new BundlesApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        String expand = "expand_example"; // String | Замена ссылок объектами с помощью expand
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip"; // String | 
        try {
            Bundle result = apiInstance.getBundleById(id, expand, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling BundlesApi#getBundleById");
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
| **acceptEncoding** | **String**|  | [optional] [default to gzip] |

### Return type

[**Bundle**](Bundle.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## getBundleComponentById

> BundleComponent getBundleComponentById(id, componentId, expand, accept, acceptEncoding)

Получить компонент

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.BundlesApi;

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

        BundlesApi apiInstance = new BundlesApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        UUID componentId = UUID.randomUUID(); // UUID | 
        String expand = "expand_example"; // String | Замена ссылок объектами с помощью expand
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip"; // String | 
        try {
            BundleComponent result = apiInstance.getBundleComponentById(id, componentId, expand, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling BundlesApi#getBundleComponentById");
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
| **componentId** | **UUID**|  | |
| **expand** | **String**| Замена ссылок объектами с помощью expand | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip] |

### Return type

[**BundleComponent**](BundleComponent.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## getBundleComponents

> BundleComponentList getBundleComponents(id, limit, offset, search, filter, expand, order, accept, acceptEncoding)

Получить компоненты Комплекта

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.BundlesApi;

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

        BundlesApi apiInstance = new BundlesApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        Integer limit = 1000; // Integer | Максимальное количество элементов в выданном списке (максимум 1000)
        Integer offset = 0; // Integer | Отступ в выданном списке
        String search = "search_example"; // String | Контекстный поиск по строковым полям сущностей
        String filter = "filter_example"; // String | Фильтрация выборки
        String expand = "expand_example"; // String | Замена ссылок объектами с помощью expand
        String order = "order_example"; // String | Сортировка
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip"; // String | 
        try {
            BundleComponentList result = apiInstance.getBundleComponents(id, limit, offset, search, filter, expand, order, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling BundlesApi#getBundleComponents");
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
| **search** | **String**| Контекстный поиск по строковым полям сущностей | [optional] |
| **filter** | **String**| Фильтрация выборки | [optional] |
| **expand** | **String**| Замена ссылок объектами с помощью expand | [optional] |
| **order** | **String**| Сортировка | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip] |

### Return type

[**BundleComponentList**](BundleComponentList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## getBundleFiles

> GetTaskFiles200Response getBundleFiles(id, limit, offset, accept, acceptEncoding)

Получить файлы Комплекта

Запрос на получение списка всех Файлов Комплекта.

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.BundlesApi;

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

        BundlesApi apiInstance = new BundlesApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        Integer limit = 1000; // Integer | Максимальное количество элементов в выданном списке (максимум 1000)
        Integer offset = 0; // Integer | Отступ в выданном списке
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip"; // String | 
        try {
            GetTaskFiles200Response result = apiInstance.getBundleFiles(id, limit, offset, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling BundlesApi#getBundleFiles");
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
| **acceptEncoding** | **String**|  | [optional] [default to gzip] |

### Return type

[**GetTaskFiles200Response**](GetTaskFiles200Response.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## getBundleImages

> GetProductImages200Response getBundleImages(id, limit, offset, fields, accept, acceptEncoding)

Получить изображения Комплекта

Запрос на получение всех Изображений Комплекта.

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.BundlesApi;

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

        BundlesApi apiInstance = new BundlesApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        Integer limit = 1000; // Integer | Максимальное количество элементов в выданном списке (максимум 1000)
        Integer offset = 0; // Integer | Отступ в выданном списке
        String fields = "minimumStock"; // String | Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - `minimumStock` — неснижаемый остаток (товар, модификация) - `downloadPermanentHref` — постоянная ссылка на изображение (платный тариф) - `stock` — остатки и себестоимость в позициях документов - `declaration` — прослеживаемость импортных товаров в позициях документов 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip"; // String | 
        try {
            GetProductImages200Response result = apiInstance.getBundleImages(id, limit, offset, fields, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling BundlesApi#getBundleImages");
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
| **fields** | **String**| Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - &#x60;minimumStock&#x60; — неснижаемый остаток (товар, модификация) - &#x60;downloadPermanentHref&#x60; — постоянная ссылка на изображение (платный тариф) - &#x60;stock&#x60; — остатки и себестоимость в позициях документов - &#x60;declaration&#x60; — прослеживаемость импортных товаров в позициях документов  | [optional] [enum: minimumStock, downloadPermanentHref, stock, declaration] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip] |

### Return type

[**GetProductImages200Response**](GetProductImages200Response.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## getBundles

> BundleList getBundles(limit, offset, search, filter, expand, order, accept, acceptEncoding)

Получить список комплектов

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.BundlesApi;

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

        BundlesApi apiInstance = new BundlesApi(defaultClient);
        Integer limit = 1000; // Integer | Максимальное количество элементов в выданном списке (максимум 1000)
        Integer offset = 0; // Integer | Отступ в выданном списке
        String search = "search_example"; // String | Контекстный поиск по строковым полям сущностей
        String filter = "filter_example"; // String | Фильтрация выборки
        String expand = "expand_example"; // String | Замена ссылок объектами с помощью expand
        String order = "order_example"; // String | Сортировка
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip"; // String | 
        try {
            BundleList result = apiInstance.getBundles(limit, offset, search, filter, expand, order, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling BundlesApi#getBundles");
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
| **acceptEncoding** | **String**|  | [optional] [default to gzip] |

### Return type

[**BundleList**](BundleList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## updateBundle

> Bundle updateBundle(id, bundle, expand, accept, acceptEncoding, contentType)

Изменить Комплект

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.BundlesApi;

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

        BundlesApi apiInstance = new BundlesApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        Bundle bundle = new Bundle(); // Bundle | 
        String expand = "expand_example"; // String | Замена ссылок объектами с помощью expand
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip"; // String | 
        String contentType = "application/json"; // String | 
        try {
            Bundle result = apiInstance.updateBundle(id, bundle, expand, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling BundlesApi#updateBundle");
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
| **bundle** | [**Bundle**](Bundle.md)|  | |
| **expand** | **String**| Замена ссылок объектами с помощью expand | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**Bundle**](Bundle.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## updateBundleComponent

> BundleComponent updateBundleComponent(id, componentId, bundleComponent, expand, accept, acceptEncoding, contentType)

Изменить компонент

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.BundlesApi;

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

        BundlesApi apiInstance = new BundlesApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        UUID componentId = UUID.randomUUID(); // UUID | 
        BundleComponent bundleComponent = new BundleComponent(); // BundleComponent | 
        String expand = "expand_example"; // String | Замена ссылок объектами с помощью expand
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip"; // String | 
        String contentType = "application/json"; // String | 
        try {
            BundleComponent result = apiInstance.updateBundleComponent(id, componentId, bundleComponent, expand, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling BundlesApi#updateBundleComponent");
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
| **componentId** | **UUID**|  | |
| **bundleComponent** | [**BundleComponent**](BundleComponent.md)|  | |
| **expand** | **String**| Замена ссылок объектами с помощью expand | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**BundleComponent**](BundleComponent.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |

