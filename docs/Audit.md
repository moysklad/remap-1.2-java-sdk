

# Audit

Контекст аудита

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID контекста аудита |  [optional] [readonly] |
|**uid** | **String** | Логин сотрудника |  [optional] [readonly] |
|**source** | **String** | Источник изменения. Известные значения описаны в AuditSourceType |  [optional] [readonly] |
|**moment** | **String** | Момент изменения |  [optional] [readonly] |
|**info** | **Map&lt;String, Object&gt;** | Краткое описание контекста |  [optional] [readonly] |
|**objectCount** | **Integer** | Количество измененных объектов |  [optional] [readonly] |
|**eventType** | **String** | Тип события. Известные значения описаны в AuditEventType |  [optional] [readonly] |
|**entityType** | **String** | Тип сущности |  [optional] [readonly] |
|**objectType** | **String** | Тип сущностей для специальных настроечных контекстов |  [optional] [readonly] |
|**supportAccess** | **Boolean** | Признак доступа поддержки от имени пользователя |  [optional] [readonly] |
|**events** | [**AuditEvents**](AuditEvents.md) |  |  [optional] |



