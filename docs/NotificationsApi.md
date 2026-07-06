# NotificationsApi

All URIs are relative to *https://api.moysklad.ru/api/remap/1.2*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getNotificationSettings**](NotificationsApi.md#getNotificationSettings) | **GET** /notification/settings | Получить настройки уведомлений |
| [**updateNotificationSettings**](NotificationsApi.md#updateNotificationSettings) | **PUT** /notification/settings | Изменить настройки уведомлений |



## getNotificationSettings

> NotificationSettings getNotificationSettings(accept, acceptEncoding)

Получить настройки уведомлений

Запрос на получение настроек уведомлений текущего пользователя

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.NotificationsApi;

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

        NotificationsApi apiInstance = new NotificationsApi(defaultClient);
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        try {
            NotificationSettings result = apiInstance.getNotificationSettings(accept, acceptEncoding);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling NotificationsApi#getNotificationSettings");
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

[**NotificationSettings**](NotificationSettings.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Успешный запрос. JSON представление настроек уведомлений |  -  |
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |


## updateNotificationSettings

> NotificationSettings updateNotificationSettings(notificationSettings, accept, acceptEncoding, contentType)

Изменить настройки уведомлений

Изменение настроек уведомлений текущего пользователя

### Example

```java
// Import classes:
import ru.moysklad.remap_1_2.ApiClient;
import ru.moysklad.remap_1_2.ApiException;
import ru.moysklad.remap_1_2.Configuration;
import ru.moysklad.remap_1_2.auth.*;
import ru.moysklad.remap_1_2.models.*;
import ru.moysklad.remap_1_2.api.NotificationsApi;

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

        NotificationsApi apiInstance = new NotificationsApi(defaultClient);
        NotificationSettings notificationSettings = new NotificationSettings(); // NotificationSettings | 
        String accept = "application/json"; // String | 
        String acceptEncoding = "gzip, deflate, br"; // String | 
        String contentType = "application/json"; // String | 
        try {
            NotificationSettings result = apiInstance.updateNotificationSettings(notificationSettings, accept, acceptEncoding, contentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling NotificationsApi#updateNotificationSettings");
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
| **notificationSettings** | [**NotificationSettings**](NotificationSettings.md)|  | |
| **accept** | **String**|  | [optional] [default to application/json;charset&#x3D;utf-8] [enum: application/json, application/json;charset=utf-8] |
| **acceptEncoding** | **String**|  | [optional] [default to gzip, deflate, br] |
| **contentType** | **String**|  | [optional] [default to application/json] [enum: application/json] |

### Return type

[**NotificationSettings**](NotificationSettings.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, text/html;charset=UTF-8


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Настройки уведомлений успешно обновлены |  -  |
| **0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

