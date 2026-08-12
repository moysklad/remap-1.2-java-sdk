# ReportsApi

All URIs are relative to *https://api.moysklad.ru/api/remap/1.2*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getReportDashboardDay**](ReportsApi.md#getReportDashboardDay) | **GET** /report/dashboard/day | Получить показатели за день |
| [**getReportDashboardMonth**](ReportsApi.md#getReportDashboardMonth) | **GET** /report/dashboard/month | Получить показатели за месяц |
| [**getReportDashboardWeek**](ReportsApi.md#getReportDashboardWeek) | **GET** /report/dashboard/week | Получить показатели за неделю |
| [**getReportOrdersPlotSeries**](ReportsApi.md#getReportOrdersPlotSeries) | **GET** /report/orders/plotseries | Получить показатели заказов |
| [**getReportSalesPlotSeries**](ReportsApi.md#getReportSalesPlotSeries) | **GET** /report/sales/plotseries | Получить показатели продаж |



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
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |


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
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |


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
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |


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
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |


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
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

