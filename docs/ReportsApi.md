# ReportsApi

All URIs are relative to *https://api.moysklad.ru/api/remap/1.2*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getReportCounterparty**](ReportsApi.md#getReportCounterparty) | **GET** /report/counterparty | Получить показатели контрагентов |
| [**getReportCounterpartyById**](ReportsApi.md#getReportCounterpartyById) | **GET** /report/counterparty/{id} | Получить показатели контрагента |
| [**getReportDashboardDay**](ReportsApi.md#getReportDashboardDay) | **GET** /report/dashboard/day | Получить показатели за день |
| [**getReportDashboardMonth**](ReportsApi.md#getReportDashboardMonth) | **GET** /report/dashboard/month | Получить показатели за месяц |
| [**getReportDashboardWeek**](ReportsApi.md#getReportDashboardWeek) | **GET** /report/dashboard/week | Получить показатели за неделю |
| [**getReportMoneyByAccount**](ReportsApi.md#getReportMoneyByAccount) | **GET** /report/money/byaccount | Получить остатки денежных средств по кассам и счетам |
| [**getReportMoneyPlotSeries**](ReportsApi.md#getReportMoneyPlotSeries) | **GET** /report/money/plotseries | Получить график движения денежных средств |
| [**getReportOrdersPlotSeries**](ReportsApi.md#getReportOrdersPlotSeries) | **GET** /report/orders/plotseries | Получить показатели заказов |
| [**getReportProfitByCounterparty**](ReportsApi.md#getReportProfitByCounterparty) | **GET** /report/profit/bycounterparty | Получить прибыльность по покупателям |
| [**getReportProfitByEmployee**](ReportsApi.md#getReportProfitByEmployee) | **GET** /report/profit/byemployee | Получить прибыльность по сотрудникам |
| [**getReportProfitByProduct**](ReportsApi.md#getReportProfitByProduct) | **GET** /report/profit/byproduct | Получить прибыльность по товарам |
| [**getReportProfitBySalesChannel**](ReportsApi.md#getReportProfitBySalesChannel) | **GET** /report/profit/bysaleschannel | Получить прибыльность по каналам продаж |
| [**getReportProfitByVariant**](ReportsApi.md#getReportProfitByVariant) | **GET** /report/profit/byvariant | Получить прибыльность по модификациям |
| [**getReportSalesPlotSeries**](ReportsApi.md#getReportSalesPlotSeries) | **GET** /report/sales/plotseries | Получить показатели продаж |
| [**getReportTurnoverAll**](ReportsApi.md#getReportTurnoverAll) | **GET** /report/turnover/all | Получить Обороты по товарам |
| [**getReportTurnoverByOperations**](ReportsApi.md#getReportTurnoverByOperations) | **GET** /report/turnover/byoperations | Получить Обороты по товару с детализацией по документам |
| [**getReportTurnoverByStore**](ReportsApi.md#getReportTurnoverByStore) | **GET** /report/turnover/bystore | Получить Обороты по товару с детализацией по складам |
| [**queryReportCounterparty**](ReportsApi.md#queryReportCounterparty) | **POST** /report/counterparty | Получить выборочные показатели контрагентов |



## getReportCounterparty

> ReportCounterpartyList getReportCounterparty(limit, offset, filter, accept, acceptEncoding)

Получить показатели контрагентов

Запрос отчета «Показатели контрагентов» по всем контрагентам.

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.ReportsApi;

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

        ReportsApi apiInstance = new ReportsApi(defaultClient);
        Integer limit = 1000; // Integer | Максимальное количество элементов в выданном списке (максимум 1000)
        Integer offset = 0; // Integer | Отступ в выданном списке
        String filter = "filter_example"; // String | Фильтрация выборки
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            ReportCounterpartyList result = apiInstance.getReportCounterparty(limit, offset, filter, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ReportsApi#getReportCounterparty");
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
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |

### Return type

[**ReportCounterpartyList**](ReportCounterpartyList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос. Результат - JSON представление отчета по контрагентам |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## getReportCounterpartyById

> ReportCounterparty getReportCounterpartyById(id, accept, acceptEncoding)

Получить показатели контрагента

Запрос отчета «Показатели контрагентов» по контрагенту с указанным id.

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.ReportsApi;

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

        ReportsApi apiInstance = new ReportsApi(defaultClient);
        UUID id = UUID.randomUUID(); // UUID | ID сущности
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            ReportCounterparty result = apiInstance.getReportCounterpartyById(id, accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ReportsApi#getReportCounterpartyById");
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

[**ReportCounterparty**](ReportCounterparty.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос. Результат - JSON представление отчета по контрагенту |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## getReportDashboardDay

> ReportDashboard getReportDashboardDay(accept, acceptEncoding)

Получить показатели за день

Запрос показателей за день. Для доступа к отчету требуется право на просмотр показателей &#x60;viewDashboard&#x60;. 

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.ReportsApi;

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

        ReportsApi apiInstance = new ReportsApi(defaultClient);
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            ReportDashboard result = apiInstance.getReportDashboardDay(accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ReportsApi#getReportDashboardDay");
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

[**ReportDashboard**](ReportDashboard.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос. JSON представление показателей за день |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## getReportDashboardMonth

> ReportDashboard getReportDashboardMonth(accept, acceptEncoding)

Получить показатели за месяц

Запрос показателей за месяц. Для доступа к отчету требуется право на просмотр показателей &#x60;viewDashboard&#x60;. 

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.ReportsApi;

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

        ReportsApi apiInstance = new ReportsApi(defaultClient);
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            ReportDashboard result = apiInstance.getReportDashboardMonth(accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ReportsApi#getReportDashboardMonth");
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

[**ReportDashboard**](ReportDashboard.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос. JSON представление показателей за месяц |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## getReportDashboardWeek

> ReportDashboard getReportDashboardWeek(accept, acceptEncoding)

Получить показатели за неделю

Запрос показателей за неделю. Для доступа к отчету требуется право на просмотр показателей &#x60;viewDashboard&#x60;. 

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.ReportsApi;

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

        ReportsApi apiInstance = new ReportsApi(defaultClient);
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            ReportDashboard result = apiInstance.getReportDashboardWeek(accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ReportsApi#getReportDashboardWeek");
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

[**ReportDashboard**](ReportDashboard.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос. JSON представление показателей за неделю |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## getReportMoneyByAccount

> ReportMoneyByAccountList getReportMoneyByAccount(accept, acceptEncoding)

Получить остатки денежных средств по кассам и счетам

Запрос текущих остатков денежных средств по кассам и счетам организаций. Для доступа к отчету требуется право на просмотр показателей &#x60;viewDashboard&#x60; и право «Видеть остатки денег» &#x60;viewMoneyDashboard&#x60;. 

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.ReportsApi;

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

        ReportsApi apiInstance = new ReportsApi(defaultClient);
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            ReportMoneyByAccountList result = apiInstance.getReportMoneyByAccount(accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ReportsApi#getReportMoneyByAccount");
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

[**ReportMoneyByAccountList**](ReportMoneyByAccountList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос. JSON представление отчета об остатках денежных средств |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## getReportMoneyPlotSeries

> ReportMoneyPlotSeries getReportMoneyPlotSeries(momentFrom, momentTo, interval, filter, accept, acceptEncoding, xLognexAcceptTimezone)

Получить график движения денежных средств

Запрос отчета о движении денежных средств за период с разбивкой по часам, дням или месяцам. Для доступа к отчету требуется право на просмотр показателей &#x60;viewDashboard&#x60; и право «Видеть остатки денег» &#x60;viewMoneyDashboard&#x60;. 

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.ReportsApi;

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

        ReportsApi apiInstance = new ReportsApi(defaultClient);
        String momentFrom = "momentFrom_example"; // String | Начало периода отчета в формате YYYY-MM-DD HH:MM:SS
        String momentTo = "momentTo_example"; // String | Конец периода отчета в формате YYYY-MM-DD HH:MM:SS
        String interval = "hour"; // String | Интервал построения отчета
        String filter = "filter_example"; // String | Фильтрация выборки
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String xLognexAcceptTimezone = "xLognexAcceptTimezone_example"; // String | Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: `Wed, 16 Aug 2017 23:07:01 +0700`. При подсчете показателей даты операций смещаются в таймзону клиента. 
        try {
            ReportMoneyPlotSeries result = apiInstance.getReportMoneyPlotSeries(momentFrom, momentTo, interval, filter, accept, acceptEncoding, xLognexAcceptTimezone);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ReportsApi#getReportMoneyPlotSeries");
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
| **momentFrom** | **String**| Начало периода отчета в формате YYYY-MM-DD HH:MM:SS | |
| **momentTo** | **String**| Конец периода отчета в формате YYYY-MM-DD HH:MM:SS | |
| **interval** | **String**| Интервал построения отчета | [enum: hour, day, month] |
| **filter** | **String**| Фильтрация выборки | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **xLognexAcceptTimezone** | **String**| Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;. При подсчете показателей даты операций смещаются в таймзону клиента.  | [optional] |

### Return type

[**ReportMoneyPlotSeries**](ReportMoneyPlotSeries.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос. JSON представление отчета о движении денежных средств |  * X-Lognex-Content-Timezone - Заголовок ответа. В нем указывается (как думает сервер) текущая дата на клиенте в RFC 3522. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;.  <br>  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## getReportOrdersPlotSeries

> ReportOrdersPlotSeriesList getReportOrdersPlotSeries(momentFrom, momentTo, interval, filter, accept, acceptEncoding, xLognexAcceptTimezone)

Получить показатели заказов

Запрос показателей заказов покупателей за период с разбивкой по часам, дням или месяцам. Для доступа к отчету требуется право на просмотр показателей &#x60;viewDashboard&#x60;. 

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.ReportsApi;

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

        ReportsApi apiInstance = new ReportsApi(defaultClient);
        String momentFrom = "momentFrom_example"; // String | Начало периода отчета в формате YYYY-MM-DD HH:MM:SS
        String momentTo = "momentTo_example"; // String | Конец периода отчета в формате YYYY-MM-DD HH:MM:SS
        String interval = "hour"; // String | Интервал построения отчета
        String filter = "filter_example"; // String | Фильтрация показателей заказов. Доступные поля: `organization`, `store`, `project`. Можно указать несколько значений; пустые значения недопустимы. 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String xLognexAcceptTimezone = "xLognexAcceptTimezone_example"; // String | Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: `Wed, 16 Aug 2017 23:07:01 +0700`. При подсчете показателей даты операций смещаются в таймзону клиента. 
        try {
            ReportOrdersPlotSeriesList result = apiInstance.getReportOrdersPlotSeries(momentFrom, momentTo, interval, filter, accept, acceptEncoding, xLognexAcceptTimezone);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ReportsApi#getReportOrdersPlotSeries");
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
| **momentFrom** | **String**| Начало периода отчета в формате YYYY-MM-DD HH:MM:SS | |
| **momentTo** | **String**| Конец периода отчета в формате YYYY-MM-DD HH:MM:SS | |
| **interval** | **String**| Интервал построения отчета | [enum: hour, day, month] |
| **filter** | **String**| Фильтрация показателей заказов. Доступные поля: &#x60;organization&#x60;, &#x60;store&#x60;, &#x60;project&#x60;. Можно указать несколько значений; пустые значения недопустимы.  | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **xLognexAcceptTimezone** | **String**| Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;. При подсчете показателей даты операций смещаются в таймзону клиента.  | [optional] |

### Return type

[**ReportOrdersPlotSeriesList**](ReportOrdersPlotSeriesList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос. JSON представление отчета показателей заказов |  * X-Lognex-Content-Timezone - Заголовок ответа. В нем указывается (как думает сервер) текущая дата на клиенте в RFC 3522. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;.  <br>  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## getReportProfitByCounterparty

> ReportProfitByCounterpartyList getReportProfitByCounterparty(limit, offset, filter, momentFrom, momentTo, accept, acceptEncoding, xLognexAcceptTimezone)

Получить прибыльность по покупателям

Запрос отчета «Прибыльность по покупателям». Для доступа к отчету требуется право на просмотр отчета «Прибыльность». 

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.ReportsApi;

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

        ReportsApi apiInstance = new ReportsApi(defaultClient);
        Integer limit = 1000; // Integer | Максимальное количество элементов в выданном списке (максимум 1000)
        Integer offset = 0; // Integer | Отступ в выданном списке
        String filter = "filter_example"; // String | Фильтрация выборки
        String momentFrom = "momentFrom_example"; // String | Начало периода отчета в формате YYYY-MM-DD HH:MM:SS
        String momentTo = "momentTo_example"; // String | Конец периода отчета в формате YYYY-MM-DD HH:MM:SS
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String xLognexAcceptTimezone = "xLognexAcceptTimezone_example"; // String | Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: `Wed, 16 Aug 2017 23:07:01 +0700`. При подсчете показателей даты операций смещаются в таймзону клиента. 
        try {
            ReportProfitByCounterpartyList result = apiInstance.getReportProfitByCounterparty(limit, offset, filter, momentFrom, momentTo, accept, acceptEncoding, xLognexAcceptTimezone);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ReportsApi#getReportProfitByCounterparty");
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
| **momentFrom** | **String**| Начало периода отчета в формате YYYY-MM-DD HH:MM:SS | [optional] |
| **momentTo** | **String**| Конец периода отчета в формате YYYY-MM-DD HH:MM:SS | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **xLognexAcceptTimezone** | **String**| Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;. При подсчете показателей даты операций смещаются в таймзону клиента.  | [optional] |

### Return type

[**ReportProfitByCounterpartyList**](ReportProfitByCounterpartyList.md)

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


## getReportProfitByEmployee

> ReportProfitByEmployeeList getReportProfitByEmployee(limit, offset, filter, momentFrom, momentTo, accept, acceptEncoding, xLognexAcceptTimezone)

Получить прибыльность по сотрудникам

Запрос отчета «Прибыльность по сотрудникам». Для доступа к отчету требуется право на просмотр отчета «Прибыльность». 

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.ReportsApi;

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

        ReportsApi apiInstance = new ReportsApi(defaultClient);
        Integer limit = 1000; // Integer | Максимальное количество элементов в выданном списке (максимум 1000)
        Integer offset = 0; // Integer | Отступ в выданном списке
        String filter = "filter_example"; // String | Фильтрация выборки
        String momentFrom = "momentFrom_example"; // String | Начало периода отчета в формате YYYY-MM-DD HH:MM:SS
        String momentTo = "momentTo_example"; // String | Конец периода отчета в формате YYYY-MM-DD HH:MM:SS
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String xLognexAcceptTimezone = "xLognexAcceptTimezone_example"; // String | Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: `Wed, 16 Aug 2017 23:07:01 +0700`. При подсчете показателей даты операций смещаются в таймзону клиента. 
        try {
            ReportProfitByEmployeeList result = apiInstance.getReportProfitByEmployee(limit, offset, filter, momentFrom, momentTo, accept, acceptEncoding, xLognexAcceptTimezone);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ReportsApi#getReportProfitByEmployee");
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
| **momentFrom** | **String**| Начало периода отчета в формате YYYY-MM-DD HH:MM:SS | [optional] |
| **momentTo** | **String**| Конец периода отчета в формате YYYY-MM-DD HH:MM:SS | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **xLognexAcceptTimezone** | **String**| Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;. При подсчете показателей даты операций смещаются в таймзону клиента.  | [optional] |

### Return type

[**ReportProfitByEmployeeList**](ReportProfitByEmployeeList.md)

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


## getReportProfitByProduct

> ReportProfitByProductList getReportProfitByProduct(limit, offset, filter, momentFrom, momentTo, accept, acceptEncoding, xLognexAcceptTimezone)

Получить прибыльность по товарам

Запрос отчета «Прибыльность по товарам». В отчете учитываются товары, услуги и комплекты. Для доступа к отчету требуется право на просмотр отчета «Прибыльность». 

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.ReportsApi;

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

        ReportsApi apiInstance = new ReportsApi(defaultClient);
        Integer limit = 1000; // Integer | Максимальное количество элементов в выданном списке (максимум 1000)
        Integer offset = 0; // Integer | Отступ в выданном списке
        String filter = "filter_example"; // String | Фильтрация выборки
        String momentFrom = "momentFrom_example"; // String | Начало периода отчета в формате YYYY-MM-DD HH:MM:SS
        String momentTo = "momentTo_example"; // String | Конец периода отчета в формате YYYY-MM-DD HH:MM:SS
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String xLognexAcceptTimezone = "xLognexAcceptTimezone_example"; // String | Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: `Wed, 16 Aug 2017 23:07:01 +0700`. При подсчете показателей даты операций смещаются в таймзону клиента. 
        try {
            ReportProfitByProductList result = apiInstance.getReportProfitByProduct(limit, offset, filter, momentFrom, momentTo, accept, acceptEncoding, xLognexAcceptTimezone);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ReportsApi#getReportProfitByProduct");
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
| **momentFrom** | **String**| Начало периода отчета в формате YYYY-MM-DD HH:MM:SS | [optional] |
| **momentTo** | **String**| Конец периода отчета в формате YYYY-MM-DD HH:MM:SS | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **xLognexAcceptTimezone** | **String**| Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;. При подсчете показателей даты операций смещаются в таймзону клиента.  | [optional] |

### Return type

[**ReportProfitByProductList**](ReportProfitByProductList.md)

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


## getReportProfitBySalesChannel

> ReportProfitBySalesChannelList getReportProfitBySalesChannel(limit, offset, filter, momentFrom, momentTo, accept, acceptEncoding, xLognexAcceptTimezone)

Получить прибыльность по каналам продаж

Запрос отчета «Прибыльность по каналам продаж». Для доступа к отчету требуется право на просмотр отчета «Прибыльность». 

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.ReportsApi;

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

        ReportsApi apiInstance = new ReportsApi(defaultClient);
        Integer limit = 1000; // Integer | Максимальное количество элементов в выданном списке (максимум 1000)
        Integer offset = 0; // Integer | Отступ в выданном списке
        String filter = "filter_example"; // String | Фильтрация выборки
        String momentFrom = "momentFrom_example"; // String | Начало периода отчета в формате YYYY-MM-DD HH:MM:SS
        String momentTo = "momentTo_example"; // String | Конец периода отчета в формате YYYY-MM-DD HH:MM:SS
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String xLognexAcceptTimezone = "xLognexAcceptTimezone_example"; // String | Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: `Wed, 16 Aug 2017 23:07:01 +0700`. При подсчете показателей даты операций смещаются в таймзону клиента. 
        try {
            ReportProfitBySalesChannelList result = apiInstance.getReportProfitBySalesChannel(limit, offset, filter, momentFrom, momentTo, accept, acceptEncoding, xLognexAcceptTimezone);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ReportsApi#getReportProfitBySalesChannel");
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
| **momentFrom** | **String**| Начало периода отчета в формате YYYY-MM-DD HH:MM:SS | [optional] |
| **momentTo** | **String**| Конец периода отчета в формате YYYY-MM-DD HH:MM:SS | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **xLognexAcceptTimezone** | **String**| Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;. При подсчете показателей даты операций смещаются в таймзону клиента.  | [optional] |

### Return type

[**ReportProfitBySalesChannelList**](ReportProfitBySalesChannelList.md)

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


## getReportProfitByVariant

> ReportProfitByVariantList getReportProfitByVariant(limit, offset, filter, momentFrom, momentTo, accept, acceptEncoding, xLognexAcceptTimezone)

Получить прибыльность по модификациям

Запрос отчета «Прибыльность по модификациям». В отчете учитываются модификации, товары, услуги и комплекты. Для доступа к отчету требуется право на просмотр отчета «Прибыльность». 

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.ReportsApi;

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

        ReportsApi apiInstance = new ReportsApi(defaultClient);
        Integer limit = 1000; // Integer | Максимальное количество элементов в выданном списке (максимум 1000)
        Integer offset = 0; // Integer | Отступ в выданном списке
        String filter = "filter_example"; // String | Фильтрация выборки
        String momentFrom = "momentFrom_example"; // String | Начало периода отчета в формате YYYY-MM-DD HH:MM:SS
        String momentTo = "momentTo_example"; // String | Конец периода отчета в формате YYYY-MM-DD HH:MM:SS
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String xLognexAcceptTimezone = "xLognexAcceptTimezone_example"; // String | Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: `Wed, 16 Aug 2017 23:07:01 +0700`. При подсчете показателей даты операций смещаются в таймзону клиента. 
        try {
            ReportProfitByVariantList result = apiInstance.getReportProfitByVariant(limit, offset, filter, momentFrom, momentTo, accept, acceptEncoding, xLognexAcceptTimezone);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ReportsApi#getReportProfitByVariant");
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
| **momentFrom** | **String**| Начало периода отчета в формате YYYY-MM-DD HH:MM:SS | [optional] |
| **momentTo** | **String**| Конец периода отчета в формате YYYY-MM-DD HH:MM:SS | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **xLognexAcceptTimezone** | **String**| Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;. При подсчете показателей даты операций смещаются в таймзону клиента.  | [optional] |

### Return type

[**ReportProfitByVariantList**](ReportProfitByVariantList.md)

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


## getReportSalesPlotSeries

> ReportSalesPlotSeriesList getReportSalesPlotSeries(momentFrom, momentTo, interval, filter, accept, acceptEncoding, xLognexAcceptTimezone)

Получить показатели продаж

Запрос показателей продаж за период с разбивкой по часам, дням или месяцам. В показателях продаж учитываются отгрузки, розничные продажи и полученные отчеты комиссионера. Для доступа к отчету требуется право на просмотр показателей &#x60;viewDashboard&#x60;. 

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.ReportsApi;

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

        ReportsApi apiInstance = new ReportsApi(defaultClient);
        String momentFrom = "momentFrom_example"; // String | Начало периода отчета в формате YYYY-MM-DD HH:MM:SS
        String momentTo = "momentTo_example"; // String | Конец периода отчета в формате YYYY-MM-DD HH:MM:SS
        String interval = "hour"; // String | Интервал построения отчета
        String filter = "filter_example"; // String | Фильтрация показателей продаж. Доступные поля: `organization`, `store`, `project`, `retailStore`. Можно указать несколько значений; пустые значения недопустимы. 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String xLognexAcceptTimezone = "xLognexAcceptTimezone_example"; // String | Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: `Wed, 16 Aug 2017 23:07:01 +0700`. При подсчете показателей даты операций смещаются в таймзону клиента. 
        try {
            ReportSalesPlotSeriesList result = apiInstance.getReportSalesPlotSeries(momentFrom, momentTo, interval, filter, accept, acceptEncoding, xLognexAcceptTimezone);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ReportsApi#getReportSalesPlotSeries");
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
| **momentFrom** | **String**| Начало периода отчета в формате YYYY-MM-DD HH:MM:SS | |
| **momentTo** | **String**| Конец периода отчета в формате YYYY-MM-DD HH:MM:SS | |
| **interval** | **String**| Интервал построения отчета | [enum: hour, day, month] |
| **filter** | **String**| Фильтрация показателей продаж. Доступные поля: &#x60;organization&#x60;, &#x60;store&#x60;, &#x60;project&#x60;, &#x60;retailStore&#x60;. Можно указать несколько значений; пустые значения недопустимы.  | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **xLognexAcceptTimezone** | **String**| Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;. При подсчете показателей даты операций смещаются в таймзону клиента.  | [optional] |

### Return type

[**ReportSalesPlotSeriesList**](ReportSalesPlotSeriesList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос. JSON представление отчета показателей продаж |  * X-Lognex-Content-Timezone - Заголовок ответа. В нем указывается (как думает сервер) текущая дата на клиенте в RFC 3522. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;.  <br>  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## getReportTurnoverAll

> ReportTurnoverList getReportTurnoverAll(limit, offset, filter, momentFrom, momentTo, groupBy, accept, acceptEncoding, xLognexAcceptTimezone)

Получить Обороты по товарам

Запрос отчета «Обороты по товарам» — общий отчет по оборотам товаров и модификаций.

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.ReportsApi;

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

        ReportsApi apiInstance = new ReportsApi(defaultClient);
        Integer limit = 1000; // Integer | Максимальное количество элементов в выданном списке (максимум 1000)
        Integer offset = 0; // Integer | Отступ в выданном списке
        String filter = "filter_example"; // String | Фильтрация выборки
        String momentFrom = "momentFrom_example"; // String | Начало периода отчета в формате YYYY-MM-DD HH:MM:SS
        String momentTo = "momentTo_example"; // String | Конец периода отчета в формате YYYY-MM-DD HH:MM:SS
        String groupBy = "product"; // String | Тип, по которому нужно сгруппировать выдачу. Значение по умолчанию `product`.
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String xLognexAcceptTimezone = "xLognexAcceptTimezone_example"; // String | Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: `Wed, 16 Aug 2017 23:07:01 +0700`. При подсчете показателей даты операций смещаются в таймзону клиента. 
        try {
            ReportTurnoverList result = apiInstance.getReportTurnoverAll(limit, offset, filter, momentFrom, momentTo, groupBy, accept, acceptEncoding, xLognexAcceptTimezone);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ReportsApi#getReportTurnoverAll");
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
| **momentFrom** | **String**| Начало периода отчета в формате YYYY-MM-DD HH:MM:SS | [optional] |
| **momentTo** | **String**| Конец периода отчета в формате YYYY-MM-DD HH:MM:SS | [optional] |
| **groupBy** | **String**| Тип, по которому нужно сгруппировать выдачу. Значение по умолчанию &#x60;product&#x60;. | [optional] [default to product] [enum: product, variant] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **xLognexAcceptTimezone** | **String**| Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;. При подсчете показателей даты операций смещаются в таймзону клиента.  | [optional] |

### Return type

[**ReportTurnoverList**](ReportTurnoverList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос. Результат - JSON представление отчета |  * X-Lognex-Content-Timezone - Заголовок ответа. В нем указывается (как думает сервер) текущая дата на клиенте в RFC 3522. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;.  <br>  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## getReportTurnoverByOperations

> ReportTurnoverByOperationList getReportTurnoverByOperations(filter, momentFrom, momentTo, accept, acceptEncoding, xLognexAcceptTimezone)

Получить Обороты по товару с детализацией по документам

Запрос отчета «Обороты по товару с детализацией по документам».

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.ReportsApi;

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

        ReportsApi apiInstance = new ReportsApi(defaultClient);
        String filter = "filter_example"; // String | Фильтрация выборки
        String momentFrom = "momentFrom_example"; // String | Начало периода отчета в формате YYYY-MM-DD HH:MM:SS
        String momentTo = "momentTo_example"; // String | Конец периода отчета в формате YYYY-MM-DD HH:MM:SS
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String xLognexAcceptTimezone = "xLognexAcceptTimezone_example"; // String | Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: `Wed, 16 Aug 2017 23:07:01 +0700`. При подсчете показателей даты операций смещаются в таймзону клиента. 
        try {
            ReportTurnoverByOperationList result = apiInstance.getReportTurnoverByOperations(filter, momentFrom, momentTo, accept, acceptEncoding, xLognexAcceptTimezone);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ReportsApi#getReportTurnoverByOperations");
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
| **filter** | **String**| Фильтрация выборки | [optional] |
| **momentFrom** | **String**| Начало периода отчета в формате YYYY-MM-DD HH:MM:SS | [optional] |
| **momentTo** | **String**| Конец периода отчета в формате YYYY-MM-DD HH:MM:SS | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **xLognexAcceptTimezone** | **String**| Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;. При подсчете показателей даты операций смещаются в таймзону клиента.  | [optional] |

### Return type

[**ReportTurnoverByOperationList**](ReportTurnoverByOperationList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос. Результат - JSON представление отчета |  * X-Lognex-Content-Timezone - Заголовок ответа. В нем указывается (как думает сервер) текущая дата на клиенте в RFC 3522. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;.  <br>  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## getReportTurnoverByStore

> ReportTurnoverByStoreList getReportTurnoverByStore(filter, momentFrom, momentTo, accept, acceptEncoding, xLognexAcceptTimezone)

Получить Обороты по товару с детализацией по складам

Запрос отчета «Обороты по товару с детализацией по складам».

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.ReportsApi;

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

        ReportsApi apiInstance = new ReportsApi(defaultClient);
        String filter = "filter_example"; // String | Фильтрация выборки
        String momentFrom = "momentFrom_example"; // String | Начало периода отчета в формате YYYY-MM-DD HH:MM:SS
        String momentTo = "momentTo_example"; // String | Конец периода отчета в формате YYYY-MM-DD HH:MM:SS
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String xLognexAcceptTimezone = "xLognexAcceptTimezone_example"; // String | Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: `Wed, 16 Aug 2017 23:07:01 +0700`. При подсчете показателей даты операций смещаются в таймзону клиента. 
        try {
            ReportTurnoverByStoreList result = apiInstance.getReportTurnoverByStore(filter, momentFrom, momentTo, accept, acceptEncoding, xLognexAcceptTimezone);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ReportsApi#getReportTurnoverByStore");
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
| **filter** | **String**| Фильтрация выборки | [optional] |
| **momentFrom** | **String**| Начало периода отчета в формате YYYY-MM-DD HH:MM:SS | [optional] |
| **momentTo** | **String**| Конец периода отчета в формате YYYY-MM-DD HH:MM:SS | [optional] |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **xLognexAcceptTimezone** | **String**| Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;. При подсчете показателей даты операций смещаются в таймзону клиента.  | [optional] |

### Return type

[**ReportTurnoverByStoreList**](ReportTurnoverByStoreList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос. Результат - JSON представление отчета |  * X-Lognex-Content-Timezone - Заголовок ответа. В нем указывается (как думает сервер) текущая дата на клиенте в RFC 3522. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;.  <br>  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |


## queryReportCounterparty

> ReportCounterpartyList queryReportCounterparty(reportCounterpartyQuery, accept, acceptEncoding, contentType)

Получить выборочные показатели контрагентов

Запрос отчета «Показатели контрагентов» по указанным контрагентам.

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.ReportsApi;

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

        ReportsApi apiInstance = new ReportsApi(defaultClient);
        ReportCounterpartyQuery reportCounterpartyQuery = new ReportCounterpartyQuery(); // ReportCounterpartyQuery | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            ReportCounterpartyList result = apiInstance.queryReportCounterparty(reportCounterpartyQuery, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ReportsApi#queryReportCounterparty");
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
| **reportCounterpartyQuery** | [**ReportCounterpartyQuery**](ReportCounterpartyQuery.md)|  | |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**ReportCounterpartyList**](ReportCounterpartyList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос. Результат - JSON представление отчета по указанным контрагентам |  -  |
| **0** | Ошибка запроса (тело — объект с полем errors) |  -  |

