

# CashInOperation

Элемент массива `operations` приходного ордера.  Допустимые `meta.type`: customerorder, purchasereturn, demand, invoiceout, commissionreportin, retailshift. 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID смены |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**name** | **String** | Наименование Полученного отчета комиссионера |  [optional] |
|**code** | **String** | Код Полученного отчета комиссионера |  [optional] |
|**externalCode** | **String** | Внешний код Полученного отчета комиссионера |  [optional] |
|**syncId** | **UUID** | ID синхронизации |  [optional] |
|**description** | **String** | Комментарий Полученного отчета комиссионера |  [optional] |
|**created** | **String** | Дата создания |  [optional] [readonly] |
|**deleted** | **String** | Момент последнего удаления Полученного отчета комиссионера |  [optional] [readonly] |
|**updated** | **String** | Момент последнего обновления Полученного отчета комиссионера |  [optional] [readonly] |
|**moment** | **String** | Дата документа |  [optional] |
|**deliveryPlannedMoment** | **String** | Планируемая дата приёмки |  [optional] |
|**applicable** | **Boolean** | Отметка о проведении |  [optional] |
|**printed** | **Boolean** | Напечатан ли документ |  [optional] [readonly] |
|**published** | **Boolean** | Опубликован ли документ |  [optional] [readonly] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**vatEnabled** | **Boolean** | Учитывается ли НДС |  [optional] |
|**vatIncluded** | **Boolean** | Включен ли НДС в цену |  [optional] |
|**vatSum** | **Double** | Сумма НДС |  [optional] |
|**sum** | **Double** | Сумма Полученного отчета комиссионера в копейках |  [optional] |
|**payedSum** | **Double** | Оплаченная сумма |  [optional] [readonly] |
|**shippedSum** | **Double** | Сумма отгруженного |  [optional] [readonly] |
|**reservedSum** | **Double** | Сумма товаров в резерве |  [optional] [readonly] |
|**invoicedSum** | **Double** | Сумма счетов покупателю |  [optional] [readonly] |
|**organization** | [**Organization**](Organization.md) |  |  [optional] |
|**organizationAccount** | [**Account**](Account.md) | Метаданные счета юрлица |  [optional] |
|**agent** | [**Counterparty**](Counterparty.md) |  |  [optional] |
|**agentAccount** | [**Account**](Account.md) | Метаданные счета контрагента |  [optional] |
|**store** | [**Store**](Store.md) | Метаданные склада |  [optional] |
|**state** | [**State**](State.md) | Метаданные статуса Полученного отчета комиссионера |  [optional] |
|**contract** | [**Contract**](Contract.md) | Метаданные договора |  [optional] |
|**project** | [**Project**](Project.md) | Метаданные проекта |  [optional] |
|**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива файлов |  [optional] |
|**taxSystem** | [**TaxSystemEnum**](#TaxSystemEnum) | Код системы налогообложения |  [optional] |
|**rate** | [**CurrencyRate**](CurrencyRate.md) |  |  [optional] |
|**positions** | **CommissionReportInPositionList** |  |  [optional] |
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
|**linkedSum** | **Double** | Сумма, оплаченная по данному документу |  |
|**commissionOverhead** | [**CommissionReportInCommissionOverhead**](CommissionReportInCommissionOverhead.md) |  |  [optional] |
|**commissionPeriodEnd** | **String** | Конец периода |  [optional] |
|**commissionPeriodStart** | **String** | Начало периода |  [optional] |
|**commitentSum** | **Double** | Сумма коммитента в установленной валюте |  [optional] [readonly] |
|**returnToCommissionerPositions** | **CommissionReportInReturnedPositionList** |  |  [optional] |
|**rewardPercent** | **Integer** | Процент вознаграждения |  [optional] |
|**rewardType** | **String** | Тип вознаграждения |  [optional] |



## Enum: TaxSystemEnum

| Name | Value |
|---- | -----|
| GENERAL_TAX_SYSTEM | &quot;GENERAL_TAX_SYSTEM&quot; |
| SIMPLIFIED_TAX_SYSTEM_INCOME | &quot;SIMPLIFIED_TAX_SYSTEM_INCOME&quot; |
| SIMPLIFIED_TAX_SYSTEM_INCOME_OUTCOME | &quot;SIMPLIFIED_TAX_SYSTEM_INCOME_OUTCOME&quot; |
| UNIFIED_AGRICULTURAL_TAX | &quot;UNIFIED_AGRICULTURAL_TAX&quot; |
| PRESUMPTIVE_TAX_SYSTEM | &quot;PRESUMPTIVE_TAX_SYSTEM&quot; |
| PATENT_BASED | &quot;PATENT_BASED&quot; |



