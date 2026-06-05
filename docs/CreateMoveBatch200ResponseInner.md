

# CreateMoveBatch200ResponseInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Перемещения |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**name** | **String** | Наименование Перемещения |  [optional] |
|**code** | **String** | Код Перемещения |  [optional] |
|**externalCode** | **String** | Внешний код Перемещения |  [optional] |
|**syncId** | **UUID** | ID синхронизации |  [optional] |
|**description** | **String** | Комментарий Перемещения |  [optional] |
|**created** | **String** | Дата создания |  [optional] [readonly] |
|**deleted** | **String** | Момент последнего удаления Перемещения |  [optional] [readonly] |
|**updated** | **String** | Момент последнего обновления Перемещения |  [optional] [readonly] |
|**moment** | **String** | Дата документа |  [optional] |
|**applicable** | **Boolean** | Отметка о проведении |  [optional] |
|**printed** | **Boolean** | Напечатан ли документ |  [optional] [readonly] |
|**published** | **Boolean** | Опубликован ли документ |  [optional] [readonly] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**sum** | **Double** | Сумма Перемещения в копейках |  [optional] [readonly] |
|**organization** | [**Organization**](Organization.md) |  |  [optional] |
|**sourceStore** | [**Store**](Store.md) | Метаданные склада, с которого совершается перемещение |  [optional] |
|**targetStore** | [**Store**](Store.md) | Метаданные склада, на который совершается перемещение |  [optional] |
|**state** | [**State**](State.md) | Метаданные статуса Перемещения |  [optional] |
|**project** | [**Project**](Project.md) | Метаданные проекта |  [optional] |
|**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива Файлов |  [optional] |
|**rate** | [**CurrencyRate**](CurrencyRate.md) |  |  [optional] |
|**positions** | [**MovePositionList**](MovePositionList.md) |  |  [optional] |
|**overhead** | [**Overhead**](Overhead.md) |  |  [optional] |
|**internalOrder** | [**InternalOrder**](InternalOrder.md) | Внутренний заказ, с которым связано Перемещение |  [optional] |
|**customerOrder** | [**CustomerOrder**](CustomerOrder.md) | Заказ покупателя, с которым связано Перемещение |  [optional] |
|**demand** | [**Demand**](Demand.md) | Отгрузка, связанная с Перемещением |  [optional] [readonly] |
|**supply** | [**Supply**](Supply.md) | Приемка, связанная с Перемещением |  [optional] [readonly] |
|**productionTasks** | [**List&lt;ProductionTask&gt;**](ProductionTask.md) | Связанные производственные задания |  [optional] |
|**errors** | [**List&lt;ErrorErrorsInner&gt;**](ErrorErrorsInner.md) |  |  |



