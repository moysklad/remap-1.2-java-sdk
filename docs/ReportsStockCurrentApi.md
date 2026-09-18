# ReportsStockCurrentApi

All URIs are relative to *https://api.moysklad.ru/api/remap/1.2*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getStockAllCurrent**](ReportsStockCurrentApi.md#getStockAllCurrent) | **GET** /report/stock/all/current | Получить Краткий отчет об остатках |
| [**getStockBySlotCurrent**](ReportsStockCurrentApi.md#getStockBySlotCurrent) | **GET** /report/stock/byslot/current | Получить Краткий отчет об остатках по ячейкам |
| [**getStockByStoreCurrent**](ReportsStockCurrentApi.md#getStockByStoreCurrent) | **GET** /report/stock/bystore/current | Получить Краткий отчет об остатках по складам |



## getStockAllCurrent

> List&lt;StockCurrentAll&gt; getStockAllCurrent(include, changedSince, stockType, filter, accept, acceptEncoding)

Получить Краткий отчет об остатках

Краткий отчет об остатках для частого обновления данных по номенклатуре. Возвращает один тип значения остатка, выбранный параметром &#x60;stockType&#x60;. 

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.ReportsStockCurrentApi;

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

        ReportsStockCurrentApi apiInstance = new ReportsStockCurrentApi(defaultClient);
        String include = "zeroLines"; // String | Управляет включением нулевых остатков. По умолчанию выводятся только ненулевые значения. 
        String changedSince = "changedSince_example"; // String | Выводит фактические остатки по позициям, у которых остаток изменился с указанного момента. Формат: `yyyy-MM-dd HH:mm:ss`. 
        String stockType = "stock"; // String | Тип рассчитываемого значения остатка. По умолчанию `stock`. 
        String filter = "filter_example"; // String | Фильтрация отчета по ID сущностей. Поддерживаемые поля: `assortmentId`, `storeId`. 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            List<StockCurrentAll> result = apiInstance.getStockAllCurrent(include, changedSince, stockType, filter, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ReportsStockCurrentApi#getStockAllCurrent");
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
| **include** | **String**| Управляет включением нулевых остатков. По умолчанию выводятся только ненулевые значения.  | [optional] [enum: zeroLines] |
| **changedSince** | **String**| Выводит фактические остатки по позициям, у которых остаток изменился с указанного момента. Формат: &#x60;yyyy-MM-dd HH:mm:ss&#x60;.  | [optional] |
| **stockType** | **String**| Тип рассчитываемого значения остатка. По умолчанию &#x60;stock&#x60;.  | [optional] [default to stock] [enum: stock, freeStock, quantity, reserve, inTransit] |
| **filter** | **String**| Фильтрация отчета по ID сущностей. Поддерживаемые поля: &#x60;assortmentId&#x60;, &#x60;storeId&#x60;.  | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |

### Return type

[**List&lt;StockCurrentAll&gt;**](StockCurrentAll.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос. Результат - JSON представление отчета |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## getStockBySlotCurrent

> List&lt;StockCurrentBySlot&gt; getStockBySlotCurrent(include, stockType, filter, accept, acceptEncoding)

Получить Краткий отчет об остатках по ячейкам

Краткий отчет об остатках с группировкой по номенклатуре, складам и ячейкам. Возвращает один тип значения остатка, выбранный параметром &#x60;stockType&#x60;.  Для запроса требуется фильтрация по &#x60;assortmentId&#x60; или &#x60;storeId&#x60;. 

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.ReportsStockCurrentApi;

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

        ReportsStockCurrentApi apiInstance = new ReportsStockCurrentApi(defaultClient);
        String include = "zeroLines"; // String | Управляет включением нулевых остатков. По умолчанию выводятся только ненулевые значения. 
        String stockType = "stock"; // String | Тип рассчитываемого значения остатка. По умолчанию `stock`. 
        String filter = "filter_example"; // String | Фильтрация отчета по ID сущностей. Поддерживаемые поля: `assortmentId`, `storeId`. 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            List<StockCurrentBySlot> result = apiInstance.getStockBySlotCurrent(include, stockType, filter, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ReportsStockCurrentApi#getStockBySlotCurrent");
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
| **include** | **String**| Управляет включением нулевых остатков. По умолчанию выводятся только ненулевые значения.  | [optional] [enum: zeroLines] |
| **stockType** | **String**| Тип рассчитываемого значения остатка. По умолчанию &#x60;stock&#x60;.  | [optional] [default to stock] [enum: stock, freeStock, quantity, reserve, inTransit] |
| **filter** | **String**| Фильтрация отчета по ID сущностей. Поддерживаемые поля: &#x60;assortmentId&#x60;, &#x60;storeId&#x60;.  | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |

### Return type

[**List&lt;StockCurrentBySlot&gt;**](StockCurrentBySlot.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос. Результат - JSON представление отчета |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## getStockByStoreCurrent

> List&lt;StockCurrentByStore&gt; getStockByStoreCurrent(include, changedSince, stockType, withRecalculate, filter, accept, acceptEncoding)

Получить Краткий отчет об остатках по складам

Краткий отчет об остатках с группировкой по номенклатуре и складам. Возвращает один тип значения остатка, выбранный параметром &#x60;stockType&#x60;. 

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.ReportsStockCurrentApi;

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

        ReportsStockCurrentApi apiInstance = new ReportsStockCurrentApi(defaultClient);
        String include = "zeroLines"; // String | Управляет включением нулевых остатков. По умолчанию выводятся только ненулевые значения. 
        String changedSince = "changedSince_example"; // String | Выводит фактические остатки по позициям, у которых остаток изменился с указанного момента. Формат: `yyyy-MM-dd HH:mm:ss`. 
        String stockType = "stock"; // String | Тип рассчитываемого значения остатка. По умолчанию `stock`. 
        Boolean withRecalculate = true; // Boolean | Включает позиции, по которым остаток пересчитывается. Для таких позиций значение остатка может быть `null`. 
        String filter = "filter_example"; // String | Фильтрация отчета по ID сущностей. Поддерживаемые поля: `assortmentId`, `storeId`. 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            List<StockCurrentByStore> result = apiInstance.getStockByStoreCurrent(include, changedSince, stockType, withRecalculate, filter, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ReportsStockCurrentApi#getStockByStoreCurrent");
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
| **include** | **String**| Управляет включением нулевых остатков. По умолчанию выводятся только ненулевые значения.  | [optional] [enum: zeroLines] |
| **changedSince** | **String**| Выводит фактические остатки по позициям, у которых остаток изменился с указанного момента. Формат: &#x60;yyyy-MM-dd HH:mm:ss&#x60;.  | [optional] |
| **stockType** | **String**| Тип рассчитываемого значения остатка. По умолчанию &#x60;stock&#x60;.  | [optional] [default to stock] [enum: stock, freeStock, quantity, reserve, inTransit] |
| **withRecalculate** | **Boolean**| Включает позиции, по которым остаток пересчитывается. Для таких позиций значение остатка может быть &#x60;null&#x60;.  | [optional] |
| **filter** | **String**| Фильтрация отчета по ID сущностей. Поддерживаемые поля: &#x60;assortmentId&#x60;, &#x60;storeId&#x60;.  | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |

### Return type

[**List&lt;StockCurrentByStore&gt;**](StockCurrentByStore.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос. Результат - JSON представление отчета |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |

