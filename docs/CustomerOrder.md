

# CustomerOrder

Заказ покупателя

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Заказа покупателя |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**name** | **String** | Наименование Заказа покупателя |  [optional] |
|**code** | **String** | Код Заказа покупателя |  [optional] |
|**externalCode** | **String** | Внешний код Заказа покупателя |  [optional] |
|**syncId** | **UUID** | ID синхронизации |  [optional] |
|**description** | **String** | Комментарий Заказа покупателя |  [optional] |
|**created** | **String** | Дата создания |  [optional] [readonly] |
|**deleted** | **String** | Момент последнего удаления Заказа покупателя |  [optional] [readonly] |
|**updated** | **String** | Момент последнего обновления Заказа покупателя |  [optional] [readonly] |
|**moment** | **String** | Дата документа |  [optional] |
|**deliveryPlannedMoment** | **String** | Планируемая дата приёмки |  [optional] |
|**applicable** | **Boolean** | Отметка о проведении |  [optional] |
|**printed** | **Boolean** | Напечатан ли документ |  [optional] [readonly] |
|**published** | **Boolean** | Опубликован ли документ |  [optional] [readonly] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**vatEnabled** | **Boolean** | Учитывается ли НДС |  [optional] |
|**vatIncluded** | **Boolean** | Включен ли НДС в цену |  [optional] |
|**vatSum** | **Double** | Сумма НДС |  [optional] [readonly] |
|**sum** | **Double** | Сумма Заказа в установленной валюте |  [optional] [readonly] |
|**payedSum** | **Double** | Сумма входящих платежей по Заказу |  [optional] [readonly] |
|**shippedSum** | **Double** | Сумма отгруженного |  [optional] [readonly] |
|**reservedSum** | **Double** | Сумма товаров в резерве |  [optional] [readonly] |
|**invoicedSum** | **Double** | Сумма счетов покупателю |  [optional] [readonly] |
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
|**taxSystem** | **String** | Код системы налогообложения. Известные значения описаны в TaxSystem |  [optional] |
|**rate** | [**CurrencyRate**](CurrencyRate.md) |  |  [optional] |
|**positions** | [**CustomerOrderPositionList**](CustomerOrderPositionList.md) |  |  [optional] |
|**salesChannel** | [**SalesChannel**](SalesChannel.md) | Метаданные канала продаж |  [optional] |
|**shipmentAddress** | **String** | Адрес доставки Заказа покупателя |  [optional] |
|**shipmentAddressFull** | [**Address**](Address.md) | Адрес доставки Заказа покупателя с детализацией по отдельным полям |  [optional] |
|**invoicesOut** | [**List&lt;InvoiceOut&gt;**](InvoiceOut.md) | Массив ссылок на связанные счета покупателям |  [optional] |
|**demands** | [**List&lt;Demand&gt;**](Demand.md) | Массив ссылок на связанные отгрузки |  [optional] |
|**payments** | [**List&lt;CustomerOrderPaymentsInner&gt;**](CustomerOrderPaymentsInner.md) | Массив ссылок на связанные платежи |  [optional] |
|**prepayments** | [**List&lt;Prepayment&gt;**](Prepayment.md) | Массив ссылок на связанные предоплаты |  [optional] |
|**purchaseOrders** | [**List&lt;PurchaseOrder&gt;**](PurchaseOrder.md) | Массив ссылок на связанные заказы поставщикам |  [optional] |
|**moves** | [**List&lt;Move&gt;**](Move.md) | Массив ссылок на связанные перемещения |  [optional] |
|**productionTasks** | [**List&lt;ProductionTask&gt;**](ProductionTask.md) | Массив ссылок на связанные производственные задания |  [optional] |



