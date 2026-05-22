

# CreateProcessingStagesBatch200ResponseInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Этапа производства |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**owner** | [**Employee**](Employee.md) | Метаданные владельца (Сотрудника) |  [optional] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**updated** | **String** | Момент последнего обновления Этапа производства |  [optional] [readonly] |
|**name** | **String** | Наименование Этапа производства |  [optional] |
|**description** | **String** | Комментарий Этапа производства |  [optional] |
|**externalCode** | **String** | Внешний код Этапа производства |  [optional] |
|**archived** | **Boolean** | Добавлен ли Этап производства в архив |  [optional] |
|**allPerformers** | **Boolean** | Признак доступности назначения на этап любого сотрудника |  [optional] |
|**distributionRequired** | **Boolean** | Признак видимости заданий для исполнителей в веб-приложении МойСклад Производство |  [optional] |
|**performers** | [**List&lt;Employee&gt;**](Employee.md) | Метаданные возможных исполнителей |  [optional] |
|**materialStore** | [**Store**](Store.md) | Метаданные склада материалов |  [optional] [readonly] |
|**standardHourCost** | **Double** | Стоимость нормо-часа |  [optional] |
|**errors** | [**List&lt;ErrorErrorsInner&gt;**](ErrorErrorsInner.md) |  |  |



