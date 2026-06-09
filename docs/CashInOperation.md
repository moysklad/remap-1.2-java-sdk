

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
|**agent** | [**Agent**](Agent.md) | Метаданные контрагента или юрлица |  [optional] |
|**agentAccount** | [**Account**](Account.md) | Метаданные счета контрагента |  [optional] |
|**store** | [**Store**](Store.md) | Метаданные склада |  [optional] |
|**state** | [**State**](State.md) | Метаданные статуса Полученного отчета комиссионера |  [optional] |
|**contract** | [**Contract**](Contract.md) | Метаданные договора |  [optional] |
|**project** | [**Project**](Project.md) | Метаданные проекта |  [optional] |
|**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива файлов |  [optional] |
|**taxSystem** | **String** | Код системы налогообложения. Известные значения описаны в TaxSystem |  [optional] |
|**rate** | [**CurrencyRate**](CurrencyRate.md) |  |  [optional] |
|**positions** | **CommissionReportInPositionList** |  |  [optional] |
|**salesChannel** | [**SalesChannel**](SalesChannel.md) | Метаданные канала продаж |  [optional] |
|**shipmentAddress** | **String** | Адрес доставки Отгрузки (строка). Для удаления адреса передайте пустую строку. Не поддерживается значение &#x60;null&#x60; для сброса — см. документацию по адресу доставки.  |  [optional] |
|**shipmentAddressFull** | [**Address**](Address.md) | Адрес доставки Отгрузки с детализацией по отдельным полям |  [optional] |
|**invoicesOut** | [**List&lt;InvoiceOut&gt;**](InvoiceOut.md) | Связанные счета покупателям |  [optional] |
|**demands** | [**List&lt;Demand&gt;**](Demand.md) | Массив ссылок на связанные отгрузки |  [optional] |
|**payments** | [**List&lt;CustomerOrderPaymentsInner&gt;**](CustomerOrderPaymentsInner.md) | Массив ссылок на связанные платежи |  [optional] |
|**prepayments** | [**List&lt;Prepayment&gt;**](Prepayment.md) | Массив ссылок на связанные предоплаты |  [optional] |
|**purchaseOrders** | [**List&lt;PurchaseOrder&gt;**](PurchaseOrder.md) | Массив ссылок на связанные заказы поставщикам |  [optional] |
|**moves** | [**List&lt;Move&gt;**](Move.md) | Массив ссылок на связанные перемещения |  [optional] |
|**productionTasks** | [**List&lt;ProductionTask&gt;**](ProductionTask.md) | Связанные производственные задания |  [optional] |
|**linkedSum** | **Double** | Сумма, оплаченная по данному документу |  |
|**supply** | [**Supply**](Supply.md) | Приемка, по которой произошел возврат |  [optional] |
|**factureOut** | [**FactureOut**](FactureOut.md) | Счёт-фактура выданный, с которым связана Отгрузка |  [optional] |
|**factureIn** | [**FactureIn**](FactureIn.md) | Счет-фактура полученный, с которым связан этот возврат |  [optional] |
|**overhead** | [**Overhead**](Overhead.md) |  |  [optional] |
|**customerOrder** | [**CustomerOrder**](CustomerOrder.md) | Заказ покупателя, с которым связан Счет покупателю |  [optional] |
|**returns** | [**List&lt;SalesReturn&gt;**](SalesReturn.md) | Связанные возвраты |  [optional] |
|**cargoName** | **String** | Наименование груза |  [optional] |
|**carrier** | [**Agent**](Agent.md) | Перевозчик (контрагент или юрлицо) |  [optional] |
|**consignee** | [**Agent**](Agent.md) | Грузополучатель (контрагент или юрлицо) |  [optional] |
|**goodPackQuantity** | **Integer** | Всего мест |  [optional] |
|**shippingInstructions** | **String** | Указания грузоотправителя |  [optional] |
|**stateContractId** | **String** | Идентификатор государственного контракта, договора (соглашения) |  [optional] |
|**transportFacility** | **String** | Транспортное средство |  [optional] |
|**transportFacilityNumber** | **String** | Номер автомобиля |  [optional] |
|**paymentPlannedMoment** | **String** | Планируемая дата оплаты |  [optional] |
|**commissionOverhead** | [**CommissionReportInCommissionOverhead**](CommissionReportInCommissionOverhead.md) |  |  [optional] |
|**commissionPeriodEnd** | **String** | Конец периода |  [optional] |
|**commissionPeriodStart** | **String** | Начало периода |  [optional] |
|**commitentSum** | **Double** | Сумма коммитента в установленной валюте |  [optional] [readonly] |
|**returnToCommissionerPositions** | **CommissionReportInReturnedPositionList** |  |  [optional] |
|**rewardPercent** | **Integer** | Процент вознаграждения |  [optional] |
|**rewardType** | **String** | Тип Вознаграждения. Известные значения описаны в RewardType |  [optional] |



