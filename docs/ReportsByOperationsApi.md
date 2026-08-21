# ReportsByOperationsApi

All URIs are relative to *https://api.moysklad.ru/api/remap/1.2*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getByOperationsInTransit**](ReportsByOperationsApi.md#getByOperationsInTransit) | **GET** /report/byoperations/intransit | Получить Отчет по документам, отображающий ожидание |
| [**getByOperationsReserve**](ReportsByOperationsApi.md#getByOperationsReserve) | **GET** /report/byoperations/reserve | Получить Отчет по документам, отображающий резервы |
| [**getByOperationsStock**](ReportsByOperationsApi.md#getByOperationsStock) | **GET** /report/byoperations/stock | Получить Отчет по документам, отображающий остатки |



## getByOperationsInTransit

> ByOperationsInTransitList getByOperationsInTransit(filter, limit, offset, accept, acceptEncoding)

Получить Отчет по документам, отображающий ожидание

Отчет по документам номенклатуры, формирующим ожидания. Обязательный параметр фильтрации — &#x60;filter&#x60; с полем &#x60;assortment&#x60; (ссылка на товар, модификацию или партию; только одна номенклатура). Для доступа нужны права на просмотр товаров и остатков. 

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.ReportsByOperationsApi;

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

        ReportsByOperationsApi apiInstance = new ReportsByOperationsApi(defaultClient);
        String filter = "filter_example"; // String | Фильтрация выборки. Обязательно указать `assortment=<href>` — ссылку на товар, модификацию или партию. Можно фильтровать только по одной номенклатуре. 
        Integer limit = 1000; // Integer | Максимальное количество элементов в выданном списке (максимум 1000)
        Integer offset = 0; // Integer | Отступ в выданном списке
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            ByOperationsInTransitList result = apiInstance.getByOperationsInTransit(filter, limit, offset, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ReportsByOperationsApi#getByOperationsInTransit");
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
| **filter** | **String**| Фильтрация выборки. Обязательно указать &#x60;assortment&#x3D;&lt;href&gt;&#x60; — ссылку на товар, модификацию или партию. Можно фильтровать только по одной номенклатуре.  | |
| **limit** | **Integer**| Максимальное количество элементов в выданном списке (максимум 1000) | [optional] [default to 1000] |
| **offset** | **Integer**| Отступ в выданном списке | [optional] [default to 0] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |

### Return type

[**ByOperationsInTransitList**](ByOperationsInTransitList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос. Результат - JSON представление отчета |  -  |
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |


## getByOperationsReserve

> ByOperationsReserveList getByOperationsReserve(filter, limit, offset, accept, acceptEncoding)

Получить Отчет по документам, отображающий резервы

Отчет по документам номенклатуры, формирующим резервы. Обязательный параметр фильтрации — &#x60;filter&#x60; с полем &#x60;assortment&#x60; (ссылка на товар, модификацию или партию; только одна номенклатура). Для доступа нужны права на просмотр товаров и остатков. 

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.ReportsByOperationsApi;

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

        ReportsByOperationsApi apiInstance = new ReportsByOperationsApi(defaultClient);
        String filter = "filter_example"; // String | Фильтрация выборки. Обязательно указать `assortment=<href>` — ссылку на товар, модификацию или партию. Можно фильтровать только по одной номенклатуре. 
        Integer limit = 1000; // Integer | Максимальное количество элементов в выданном списке (максимум 1000)
        Integer offset = 0; // Integer | Отступ в выданном списке
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            ByOperationsReserveList result = apiInstance.getByOperationsReserve(filter, limit, offset, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ReportsByOperationsApi#getByOperationsReserve");
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
| **filter** | **String**| Фильтрация выборки. Обязательно указать &#x60;assortment&#x3D;&lt;href&gt;&#x60; — ссылку на товар, модификацию или партию. Можно фильтровать только по одной номенклатуре.  | |
| **limit** | **Integer**| Максимальное количество элементов в выданном списке (максимум 1000) | [optional] [default to 1000] |
| **offset** | **Integer**| Отступ в выданном списке | [optional] [default to 0] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |

### Return type

[**ByOperationsReserveList**](ByOperationsReserveList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос. Результат - JSON представление отчета |  -  |
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |


## getByOperationsStock

> ByOperationsStockList getByOperationsStock(filter, limit, offset, accept, acceptEncoding)

Получить Отчет по документам, отображающий остатки

Отчет по документам номенклатуры, формирующим остатки. Обязательный параметр фильтрации — &#x60;filter&#x60; с полем &#x60;assortment&#x60; (ссылка на товар, модификацию или партию; только одна номенклатура). Для доступа нужны права на просмотр товаров и остатков. Поля себестоимости (&#x60;costPerUnit&#x60;, &#x60;sumCost&#x60;) не возвращаются без пермиссии «Видеть себестоимость, цену закупки, прибыль товаров». 

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.ReportsByOperationsApi;

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

        ReportsByOperationsApi apiInstance = new ReportsByOperationsApi(defaultClient);
        String filter = "filter_example"; // String | Фильтрация выборки. Обязательно указать `assortment=<href>` — ссылку на товар, модификацию или партию. Можно фильтровать только по одной номенклатуре. 
        Integer limit = 1000; // Integer | Максимальное количество элементов в выданном списке (максимум 1000)
        Integer offset = 0; // Integer | Отступ в выданном списке
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            ByOperationsStockList result = apiInstance.getByOperationsStock(filter, limit, offset, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ReportsByOperationsApi#getByOperationsStock");
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
| **filter** | **String**| Фильтрация выборки. Обязательно указать &#x60;assortment&#x3D;&lt;href&gt;&#x60; — ссылку на товар, модификацию или партию. Можно фильтровать только по одной номенклатуре.  | |
| **limit** | **Integer**| Максимальное количество элементов в выданном списке (максимум 1000) | [optional] [default to 1000] |
| **offset** | **Integer**| Отступ в выданном списке | [optional] [default to 0] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |

### Return type

[**ByOperationsStockList**](ByOperationsStockList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос. Результат - JSON представление отчета |  -  |
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

