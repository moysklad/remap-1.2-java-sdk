

# WebhookStockNotificationPayload

Тело HTTP POST, которое МойСклад отправляет на url вебхука при изменении остатков (уведомления с интервалом 1–5 минут). Параметр query requestId идентифицирует уведомление (сохраняется при повторных попытках). 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**accountId** | **UUID** | ID учетной записи |  [optional] |
|**stockType** | **String** | Тип остатков. Известные значения описаны в WebhookStockStockType |  [optional] |
|**reportType** | **String** | Тип отчёта. Известные значения описаны в WebhookStockReportType |  [optional] |
|**reportUrl** | **String** | URL для получения данных по изменившейся номенклатуре за период (отчёт об остатках) |  [optional] |



