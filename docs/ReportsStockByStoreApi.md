# ReportsStockByStoreApi

All URIs are relative to *https://api.moysklad.ru/api/remap/1.2*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getStockByStore**](ReportsStockByStoreApi.md#getStockByStore) | **GET** /report/stock/bystore | Получить Остатки по складам |



## getStockByStore

> StockByStoreList getStockByStore(limit, offset, filter, order, groupBy, accept, acceptEncoding)

Получить Остатки по складам

Запрос отчета «Остатки по складам» — остаток по каждому товару на каждом складе. Тип объектов в выдаче задается параметром &#x60;groupBy&#x60;: товары (product), товары и модификации (variant), товары, модификации и партии (consignment). 

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.ReportsStockByStoreApi;

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

        ReportsStockByStoreApi apiInstance = new ReportsStockByStoreApi(defaultClient);
        Integer limit = 1000; // Integer | Максимальное количество элементов в выданном списке (максимум 1000)
        Integer offset = 0; // Integer | Отступ в выданном списке
        String filter = "filter_example"; // String | Фильтрация выборки
        String order = "order_example"; // String | Сортировка
        String groupBy = "product"; // String | Тип, по которому нужно сгруппировать выдачу. Значение по умолчанию `variant`. - `product` — выдает только товары - `variant` — выдает товары и модификации - `consignment` — выдает товары, модификации, партии 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            StockByStoreList result = apiInstance.getStockByStore(limit, offset, filter, order, groupBy, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ReportsStockByStoreApi#getStockByStore");
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
| **filter** | **String**| Фильтрация выборки | [optional] |
| **order** | **String**| Сортировка | [optional] |
| **groupBy** | **String**| Тип, по которому нужно сгруппировать выдачу. Значение по умолчанию &#x60;variant&#x60;. - &#x60;product&#x60; — выдает только товары - &#x60;variant&#x60; — выдает товары и модификации - &#x60;consignment&#x60; — выдает товары, модификации, партии  | [optional] [enum: product, variant, consignment] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |

### Return type

[**StockByStoreList**](StockByStoreList.md)

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

