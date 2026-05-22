

# WebhookEvent

Элемент массива events во входящем теле уведомления вебхука

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**action** | **String** | Действие, вызвавшее срабатывание. Известные значения описаны в WebhookAction |  [optional] |
|**accountId** | **UUID** | ID учетной записи |  [optional] |
|**updatedFields** | **List&lt;String&gt;** | Поля сущности, измененные пользователем (при diffType&#x3D;FIELDS и action&#x3D;UPDATE у настройки вебхука) |  [optional] |



