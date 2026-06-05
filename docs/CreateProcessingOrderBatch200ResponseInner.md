

# CreateProcessingOrderBatch200ResponseInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID заказа на производство |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**name** | **String** | Наименование заказа на производство |  [optional] |
|**code** | **String** | Код заказа на производство |  [optional] |
|**externalCode** | **String** | Внешний код заказа на производство |  [optional] |
|**syncId** | **UUID** | ID синхронизации |  [optional] |
|**description** | **String** | Комментарий заказа на производство |  [optional] |
|**created** | **String** | Дата создания |  [optional] [readonly] |
|**deleted** | **String** | Момент последнего удаления заказа на производство |  [optional] [readonly] |
|**updated** | **String** | Момент последнего обновления заказа на производство |  [optional] [readonly] |
|**moment** | **String** | Дата документа |  [optional] |
|**deliveryPlannedMoment** | **String** | Планируемая дата производства |  [optional] |
|**applicable** | **Boolean** | Отметка о проведении |  [optional] |
|**printed** | **Boolean** | Напечатан ли документ |  [optional] [readonly] |
|**published** | **Boolean** | Опубликован ли документ |  [optional] [readonly] |
|**shared** | **Boolean** | Общий доступ |  [optional] [readonly] |
|**organization** | [**Organization**](Organization.md) |  |  [optional] |
|**store** | [**Store**](Store.md) |  |  [optional] |
|**state** | [**State**](State.md) | Метаданные статуса Заказа на производство |  [optional] |
|**processingPlan** | [**ProcessingPlan**](ProcessingPlan.md) |  |  [optional] |
|**project** | [**Project**](Project.md) | Метаданные проекта |  [optional] |
|**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива Файлов |  [optional] |
|**positions** | **ProcessingOrderPositionList** |  |  [optional] |
|**quantity** | **Double** | Объем производства |  [optional] |
|**processings** | [**List&lt;Processing&gt;**](Processing.md) | Массив ссылок на связанные техоперации |  [optional] |
|**errors** | [**List&lt;ErrorErrorsInner&gt;**](ErrorErrorsInner.md) |  |  |



