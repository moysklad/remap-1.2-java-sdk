

# CreateInternalOrderBatch200ResponseInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Внутреннего заказа |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**name** | **String** | Наименование Внутреннего заказа |  [optional] |
|**code** | **String** | Код Внутреннего заказа |  [optional] |
|**externalCode** | **String** | Внешний код Внутреннего заказа |  [optional] |
|**syncId** | **UUID** | ID синхронизации |  [optional] |
|**description** | **String** | Комментарий Внутреннего заказа |  [optional] |
|**created** | **String** | Дата создания |  [optional] [readonly] |
|**deleted** | **String** | Момент последнего удаления Внутреннего заказа |  [optional] [readonly] |
|**updated** | **String** | Момент последнего обновления Внутреннего заказа |  [optional] [readonly] |
|**moment** | **String** | Дата документа |  [optional] |
|**deliveryPlannedMoment** | **String** | Планируемая дата приемки |  [optional] |
|**applicable** | **Boolean** | Отметка о проведении |  [optional] |
|**printed** | **Boolean** | Напечатан ли документ |  [optional] [readonly] |
|**published** | **Boolean** | Опубликован ли документ |  [optional] [readonly] |
|**shared** | **Boolean** | Общий доступ |  [optional] [readonly] |
|**vatEnabled** | **Boolean** | Учитывается ли НДС |  [optional] |
|**vatIncluded** | **Boolean** | Включен ли НДС в цену |  [optional] |
|**vatSum** | **Double** | Сумма НДС |  [optional] [readonly] |
|**sum** | **Double** | Сумма Внутреннего заказа в копейках |  [optional] [readonly] |
|**organization** | [**Organization**](Organization.md) |  |  [optional] |
|**store** | [**Store**](Store.md) | Метаданные склада |  [optional] |
|**state** | [**State**](State.md) | Метаданные статуса Внутреннего заказа |  [optional] |
|**project** | [**Project**](Project.md) | Метаданные проекта |  [optional] |
|**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива Файлов |  [optional] |
|**rate** | [**CurrencyRate**](CurrencyRate.md) |  |  [optional] |
|**positions** | [**InternalOrderPositionList**](InternalOrderPositionList.md) |  |  [optional] |
|**purchaseOrders** | [**List&lt;PurchaseOrder&gt;**](PurchaseOrder.md) | Коллекция метаданных на связанные заказы поставщику |  [optional] |
|**productionTasks** | [**List&lt;ProductionTask&gt;**](ProductionTask.md) | Массив ссылок на связанные производственные задания |  [optional] |
|**moves** | [**List&lt;Move&gt;**](Move.md) | Коллекция метаданных на связанные заказы перемещения |  [optional] |
|**processingOrder** | [**ProcessingOrder**](ProcessingOrder.md) | Метаданные Заказа на производство |  [optional] |
|**errors** | [**List&lt;ErrorErrorsInner&gt;**](ErrorErrorsInner.md) |  |  |



