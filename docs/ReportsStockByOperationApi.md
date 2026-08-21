# ReportsStockByOperationApi

All URIs are relative to *https://api.moysklad.ru/api/remap/1.2*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getStockByOperation**](ReportsStockByOperationApi.md#getStockByOperation) | **GET** /report/stock/byoperation | Получить Остатки по документу |



## getStockByOperation

> StockByOperationList getStockByOperation(operationId, accept, acceptEncoding)

Получить Остатки по документу

Запрос отчета «Остатки по документам» — остатки по позициям указанного документа со склада документа, а также себестоимость позиций по FIFO с учётом количества.  Обязательный параметр — &#x60;operation.id&#x60; (ID документа).  Поддерживаемые типы документов: отгрузка, заказ покупателя, розничная продажа, счет поставщика, счет покупателю, заказ поставщику, приемка, розничный возврат, возврат поставщику, возврат покупателя.  Для отгрузки, розничной продажи, приемки, возвратов остатки рассчитываются на момент поля &#x60;moment&#x60; документа. Для заказа покупателя, счетов и заказа поставщику — на текущий момент времени. 

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.ReportsStockByOperationApi;

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

        ReportsStockByOperationApi apiInstance = new ReportsStockByOperationApi(defaultClient);
        UUID operationId = UUID.randomUUID(); // UUID | ID документа, по которому нужно получить остатки
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            StockByOperationList result = apiInstance.getStockByOperation(operationId, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ReportsStockByOperationApi#getStockByOperation");
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
| **operationId** | **UUID**| ID документа, по которому нужно получить остатки | |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |

### Return type

[**StockByOperationList**](StockByOperationList.md)

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

