

# PaymentOutOperation

Элемент массива `operations` исходящего платежа: **полноценный документ** одного из допустимых типов плюс обязательное поле `linkedSum`.  Допустимые `meta.type`: salesreturn, supply, invoicein, purchaseorder, commissionreportout 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Выданного отчета комиссионера |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**name** | **String** | Наименование Выданного отчета комиссионера |  [optional] |
|**code** | **String** | Код Выданного отчета комиссионера |  [optional] |
|**externalCode** | **String** | Внешний код Выданного отчета комиссионера |  [optional] |
|**syncId** | **UUID** | ID синхронизации |  [optional] |
|**description** | **String** | Комментарий Выданного отчета комиссионера |  [optional] |
|**created** | **String** | Дата создания |  [optional] [readonly] |
|**deleted** | **String** | Момент последнего удаления Выданного отчета комиссионера |  [optional] [readonly] |
|**updated** | **String** | Момент последнего обновления Выданного отчета комиссионера |  [optional] [readonly] |
|**moment** | **String** | Дата документа |  [optional] |
|**applicable** | **Boolean** | Отметка о проведении |  [optional] |
|**printed** | **Boolean** | Напечатан ли документ |  [optional] [readonly] |
|**published** | **Boolean** | Опубликован ли документ |  [optional] [readonly] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**vatEnabled** | **Boolean** | Учитывается ли НДС |  [optional] |
|**vatIncluded** | **Boolean** | Включен ли НДС в цену |  [optional] |
|**vatSum** | **Double** | Сумма НДС |  [optional] |
|**sum** | **Double** | Сумма Выданного отчета комиссионера в копейках |  [optional] |
|**payedSum** | **Double** | Оплаченная сумма |  [optional] [readonly] |
|**organization** | [**Organization**](Organization.md) |  |  [optional] |
|**organizationAccount** | [**Account**](Account.md) | Метаданные счета юрлица |  [optional] |
|**agent** | [**Agent**](Agent.md) | Метаданные контрагента или юрлица |  [optional] |
|**agentAccount** | [**Account**](Account.md) | Метаданные счета контрагента |  [optional] |
|**store** | [**Store**](Store.md) | Метаданные склада |  [optional] |
|**state** | [**State**](State.md) | Метаданные статуса Выданного отчета комиссионера |  [optional] |
|**contract** | [**Contract**](Contract.md) | Метаданные договора |  [optional] |
|**project** | [**Project**](Project.md) | Метаданные проекта |  [optional] |
|**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива файлов |  [optional] |
|**rate** | [**CurrencyRate**](CurrencyRate.md) |  |  [optional] |
|**positions** | **CommissionReportOutPositionList** |  |  [optional] |
|**salesChannel** | [**SalesChannel**](SalesChannel.md) | Метаданные канала продаж |  [optional] |
|**demand** | [**Demand**](Demand.md) | Отгрузка, по которой произошел возврат |  [optional] |
|**losses** | [**List&lt;Loss&gt;**](Loss.md) | Массив ссылок на связанные списания |  [optional] |
|**payments** | [**List&lt;CustomerOrderPaymentsInner&gt;**](CustomerOrderPaymentsInner.md) | Массив ссылок на связанные платежи |  [optional] |
|**factureOut** | [**FactureOut**](FactureOut.md) | Счет-фактура выданный, с которым связан этот возврат |  [optional] |
|**linkedSum** | **Double** | Сумма, оплаченная по данному документу |  |
|**incomingDate** | **String** | Входящая дата |  [optional] |
|**incomingNumber** | **String** | Входящий номер |  [optional] |
|**overhead** | [**Overhead**](Overhead.md) |  |  [optional] |
|**purchaseOrder** | [**PurchaseOrder**](PurchaseOrder.md) | Заказ поставщику, с которым связана Приемка  |  [optional] |
|**factureIn** | [**FactureIn**](FactureIn.md) | Счет-фактура полученный, с которым связана эта Приемка |  [optional] |
|**invoicesIn** | [**List&lt;InvoiceIn&gt;**](InvoiceIn.md) | Массив ссылок на связанные счета поставщиков |  [optional] |
|**productionTask** | [**ProductionTask**](ProductionTask.md) | Связанное производственное задание |  [optional] |
|**returns** | [**List&lt;SupplyReturnsInner&gt;**](SupplyReturnsInner.md) | Массив ссылок на связанные возвраты  |  [optional] |
|**deliveryPlannedMoment** | **String** | Планируемая дата отгрузки |  [optional] |
|**shippedSum** | **Double** | Сумма принятого |  [optional] [readonly] |
|**invoicedSum** | **Double** | Сумма счетов поставщику |  [optional] [readonly] |
|**waitSum** | **Double** | Сумма товаров в пути |  [optional] [readonly] |
|**internalOrder** | [**InternalOrder**](InternalOrder.md) | Внутренний заказ, связанный с заказом поставщику |  [optional] |
|**customerOrders** | [**List&lt;CustomerOrder&gt;**](CustomerOrder.md) | Массив ссылок на связанные заказы покупателей |  [optional] |
|**supplies** | [**List&lt;Supply&gt;**](Supply.md) | Массив ссылок на связанные приемки |  [optional] |
|**productionTasks** | [**List&lt;ProductionTask&gt;**](ProductionTask.md) | Массив ссылок на связанные производственные задания |  [optional] |
|**commissionPeriodEnd** | **String** | Конец периода |  [optional] |
|**commissionPeriodStart** | **String** | Начало периода |  [optional] |
|**commitentSum** | **Double** | Сумма коммитента в установленной валюте |  [optional] [readonly] |
|**rewardPercent** | **Integer** | Процент вознаграждения |  [optional] |
|**rewardType** | **String** | Тип Вознаграждения. Известные значения описаны в RewardType |  [optional] |



