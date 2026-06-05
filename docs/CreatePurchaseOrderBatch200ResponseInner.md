

# CreatePurchaseOrderBatch200ResponseInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Заказа поставщику |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**name** | **String** | Наименование Заказа поставщику |  [optional] |
|**code** | **String** | Код Заказа поставщику |  [optional] |
|**externalCode** | **String** | Внешний код Заказа поставщику |  [optional] |
|**syncId** | **UUID** | ID синхронизации |  [optional] |
|**description** | **String** | Комментарий Заказа поставщику |  [optional] |
|**created** | **String** | Дата создания |  [optional] [readonly] |
|**deleted** | **String** | Момент последнего удаления Заказа поставщику |  [optional] [readonly] |
|**updated** | **String** | Момент последнего обновления Заказа поставщику |  [optional] [readonly] |
|**moment** | **String** | Дата документа |  [optional] |
|**deliveryPlannedMoment** | **String** | Планируемая дата отгрузки |  [optional] |
|**applicable** | **Boolean** | Отметка о проведении |  [optional] |
|**printed** | **Boolean** | Напечатан ли документ |  [optional] [readonly] |
|**published** | **Boolean** | Опубликован ли документ |  [optional] [readonly] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**vatEnabled** | **Boolean** | Учитывается ли НДС |  [optional] |
|**vatIncluded** | **Boolean** | Включен ли НДС в цену |  [optional] |
|**vatSum** | **Double** | Сумма НДС |  [optional] [readonly] |
|**sum** | **Double** | Сумма Заказа поставщику в установленной валюте |  [optional] [readonly] |
|**payedSum** | **Double** | Сумма входящих платежей по Заказу |  [optional] [readonly] |
|**shippedSum** | **Double** | Сумма принятого |  [optional] [readonly] |
|**invoicedSum** | **Double** | Сумма счетов поставщику |  [optional] [readonly] |
|**waitSum** | **Double** | Сумма товаров в пути |  [optional] [readonly] |
|**organization** | [**Organization**](Organization.md) |  |  [optional] |
|**organizationAccount** | [**Account**](Account.md) | Метаданные счета юрлица |  [optional] |
|**agent** | [**Agent**](Agent.md) | Метаданные контрагента или юрлица |  [optional] |
|**agentAccount** | [**Account**](Account.md) | Метаданные счета контрагента |  [optional] |
|**store** | [**Store**](Store.md) | Метаданные склада |  [optional] |
|**state** | [**State**](State.md) | Метаданные статуса заказа |  [optional] |
|**contract** | [**Contract**](Contract.md) | Метаданные договора |  [optional] |
|**project** | [**Project**](Project.md) | Метаданные проекта |  [optional] |
|**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива Файлов |  [optional] |
|**rate** | [**PurchaseOrderRate**](PurchaseOrderRate.md) |  |  [optional] |
|**positions** | **PurchaseOrderPositionList** |  |  [optional] |
|**internalOrder** | [**InternalOrder**](InternalOrder.md) | Внутренний заказ, связанный с заказом поставщику |  [optional] |
|**customerOrders** | [**List&lt;CustomerOrder&gt;**](CustomerOrder.md) | Массив ссылок на связанные заказы покупателей |  [optional] |
|**invoicesIn** | [**List&lt;InvoiceIn&gt;**](InvoiceIn.md) | Массив ссылок на связанные счета поставщиков |  [optional] |
|**supplies** | [**List&lt;Supply&gt;**](Supply.md) | Массив ссылок на связанные приемки |  [optional] |
|**payments** | [**List&lt;SalesReturnPaymentsInner&gt;**](SalesReturnPaymentsInner.md) | Массив ссылок на связанные платежи |  [optional] |
|**productionTasks** | [**List&lt;ProductionTask&gt;**](ProductionTask.md) | Массив ссылок на связанные производственные задания |  [optional] |
|**errors** | [**List&lt;ErrorErrorsInner&gt;**](ErrorErrorsInner.md) |  |  |



