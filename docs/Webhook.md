

# Webhook

Вебхук

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID вебхука |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**entityType** | **String** | Тип сущности, к которой привязан вебхук. Известные ограничения см. в документации (нельзя webhook, discount, notes) |  [optional] |
|**url** | **URI** | URL, по которому отправляется уведомление |  [optional] |
|**method** | **String** | HTTP метод запроса к URL подписчика. Известные значения описаны в WebhookMethod |  [optional] |
|**enabled** | **Boolean** | Вебхук включен или отключен |  [optional] |
|**action** | **String** | Отслеживаемое действие. Известные значения описаны в WebhookAction. Значение PROCESSED допустимо только для асинхронных задач |  [optional] |
|**diffType** | **String** | Режим для действия UPDATE. Известные значения описаны в WebhookDiffType |  [optional] |
|**authorApplication** | [**Application**](Application.md) |  |  [optional] |



