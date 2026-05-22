

# WebhookNotificationPayload

Тело HTTP POST, которое МойСклад отправляет на url вебхука при событии. Параметр query requestId идентифицирует уведомление (сохраняется при повторных попытках). 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**auditContext** | [**WebhookAuditContext**](WebhookAuditContext.md) |  |  [optional] |
|**events** | [**List&lt;WebhookEvent&gt;**](WebhookEvent.md) | Данные о событии или нескольких событиях |  [optional] |



