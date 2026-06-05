

# CashInOperationAnyOf2

Отгрузка + linkedSum

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Отгрузки |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**name** | **String** | Наименование Отгрузки |  [optional] |
|**code** | **String** | Код Отгрузки |  [optional] |
|**externalCode** | **String** | Внешний код Отгрузки |  [optional] |
|**syncId** | **UUID** | ID синхронизации |  [optional] |
|**description** | **String** | Комментарий Отгрузки |  [optional] |
|**created** | **String** | Дата создания |  [optional] [readonly] |
|**deleted** | **String** | Момент последнего удаления Отгрузки |  [optional] [readonly] |
|**updated** | **String** | Момент последнего обновления Отгрузки |  [optional] [readonly] |
|**moment** | **String** | Дата документа |  [optional] |
|**applicable** | **Boolean** | Отметка о проведении |  [optional] |
|**printed** | **Boolean** | Напечатан ли документ |  [optional] [readonly] |
|**published** | **Boolean** | Опубликован ли документ |  [optional] [readonly] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**vatEnabled** | **Boolean** | Учитывается ли НДС |  [optional] |
|**vatIncluded** | **Boolean** | Включён ли НДС в цену |  [optional] |
|**vatSum** | **Double** | Сумма НДС |  [optional] [readonly] |
|**sum** | **Double** | Сумма Отгрузки в копейках |  [optional] [readonly] |
|**payedSum** | **Double** | Сумма входящих платежей по Отгрузке |  [optional] [readonly] |
|**organization** | [**Organization**](Organization.md) |  |  [optional] |
|**organizationAccount** | [**Account**](Account.md) | Метаданные счета юрлица |  [optional] |
|**agent** | [**Agent**](Agent.md) | Метаданные контрагента или юрлица |  [optional] |
|**agentAccount** | [**Account**](Account.md) | Метаданные счета контрагента |  [optional] |
|**store** | [**Store**](Store.md) | Метаданные склада |  [optional] |
|**state** | [**State**](State.md) | Метаданные статуса Отгрузки |  [optional] |
|**contract** | [**Contract**](Contract.md) | Метаданные договора |  [optional] |
|**project** | [**Project**](Project.md) | Метаданные проекта |  [optional] |
|**owner** | [**Employee**](Employee.md) | Владелец (сотрудник) |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива файлов |  [optional] |
|**rate** | [**CurrencyRate**](CurrencyRate.md) |  |  [optional] |
|**positions** | [**DemandPositionList**](DemandPositionList.md) |  |  [optional] |
|**salesChannel** | [**SalesChannel**](SalesChannel.md) | Метаданные канала продаж |  [optional] |
|**shipmentAddress** | **String** | Адрес доставки Отгрузки (строка). Для удаления адреса передайте пустую строку. Не поддерживается значение &#x60;null&#x60; для сброса — см. документацию по адресу доставки.  |  [optional] |
|**shipmentAddressFull** | [**Address**](Address.md) | Адрес доставки Отгрузки с детализацией по отдельным полям |  [optional] |
|**overhead** | [**Overhead**](Overhead.md) |  |  [optional] |
|**customerOrder** | [**CustomerOrder**](CustomerOrder.md) | Заказ покупателя, с которым связана Отгрузка |  [optional] |
|**factureOut** | [**FactureOut**](FactureOut.md) | Счёт-фактура выданный, с которым связана Отгрузка |  [optional] |
|**returns** | [**List&lt;SalesReturn&gt;**](SalesReturn.md) | Связанные возвраты |  [optional] |
|**payments** | [**List&lt;CustomerOrderPaymentsInner&gt;**](CustomerOrderPaymentsInner.md) | Связанные платежи |  [optional] |
|**productionTasks** | [**List&lt;ProductionTask&gt;**](ProductionTask.md) | Связанные производственные задания |  [optional] |
|**invoicesOut** | [**List&lt;InvoiceOut&gt;**](InvoiceOut.md) | Связанные счета покупателям |  [optional] |
|**cargoName** | **String** | Наименование груза |  [optional] |
|**carrier** | [**Agent**](Agent.md) | Перевозчик (контрагент или юрлицо) |  [optional] |
|**consignee** | [**Agent**](Agent.md) | Грузополучатель (контрагент или юрлицо) |  [optional] |
|**goodPackQuantity** | **Integer** | Всего мест |  [optional] |
|**shippingInstructions** | **String** | Указания грузоотправителя |  [optional] |
|**stateContractId** | **String** | Идентификатор государственного контракта, договора (соглашения) |  [optional] |
|**transportFacility** | **String** | Транспортное средство |  [optional] |
|**transportFacilityNumber** | **String** | Номер автомобиля |  [optional] |
|**linkedSum** | **Double** | Сумма, оплаченная по данному документу |  |



