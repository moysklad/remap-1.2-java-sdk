

# AuditEvent

Событие аудита

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**additionalInfo** | **String** | Дополнительная информация о событии |  [optional] [readonly] |
|**audit** | [**AuditEventAudit**](AuditEventAudit.md) |  |  [optional] |
|**diff** | **Map&lt;String, Object&gt;** | Изменения, произошедшие в событии |  [optional] [readonly] |
|**entity** | [**AuditEventEntity**](AuditEventEntity.md) |  |  [optional] |
|**entityType** | **String** | Тип сущности |  [optional] [readonly] |
|**eventType** | **String** | Действие события. Известные значения описаны в AuditEventType |  [optional] [readonly] |
|**moment** | **String** | Время создания события |  [optional] [readonly] |
|**name** | **String** | Имя сущности |  [optional] [readonly] |
|**objectCount** | **Integer** | Количество измененных объектов |  [optional] [readonly] |
|**objectType** | **String** | Тип сущностей для специальных настроечных событий |  [optional] [readonly] |
|**source** | **String** | Источник изменения. Известные значения описаны в AuditSourceType |  [optional] [readonly] |
|**supportAccess** | **Boolean** | Признак доступа поддержки от имени пользователя |  [optional] [readonly] |
|**uid** | **String** | Логин сотрудника |  [optional] [readonly] |



