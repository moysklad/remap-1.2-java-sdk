

# CreateOrUpdateWebhookStocksBatch200ResponseInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID вебхука на изменение остатков |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**stockType** | **String** | Тип остатков. Известные значения описаны в WebhookStockStockType |  [optional] |
|**reportType** | **String** | Тип отчёта остатков. Известные значения описаны в WebhookStockReportType |  [optional] |
|**url** | **URI** | URL, по которому будет происходить обработка вебхука |  [optional] |
|**enabled** | **Boolean** | Вебхук включён или отключён |  [optional] |
|**authorApplication** | [**Application**](Application.md) |  |  [optional] |
|**errors** | [**List&lt;ErrorErrorsInner&gt;**](ErrorErrorsInner.md) |  |  |



