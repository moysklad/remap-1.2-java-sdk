

# PaymentOutOperationAnyOf1

Приемка + linkedSum

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Приемки |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**name** | **String** | Наименование Приемки |  [optional] |
|**code** | **String** | Код Приемки |  [optional] |
|**externalCode** | **String** | Внешний код Приемки |  [optional] |
|**syncId** | **UUID** | ID синхронизации. После заполнения недоступен для изменения |  [optional] |
|**description** | **String** | Комментарий Приемки |  [optional] |
|**created** | **String** | Дата создания |  [optional] [readonly] |
|**deleted** | **String** | Момент последнего удаления Приемки |  [optional] [readonly] |
|**updated** | **String** | Момент последнего обновления Приемки |  [optional] [readonly] |
|**moment** | **String** | Дата документа |  [optional] |
|**incomingDate** | **String** | Входящая дата |  [optional] |
|**incomingNumber** | **String** | Входящий номер |  [optional] |
|**applicable** | **Boolean** | Отметка о проведении |  [optional] |
|**printed** | **Boolean** | Напечатан ли документ |  [optional] [readonly] |
|**published** | **Boolean** | Опубликован ли документ |  [optional] [readonly] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**vatEnabled** | **Boolean** | Учитывается ли НДС |  [optional] |
|**vatIncluded** | **Boolean** | Включен ли НДС в цену |  [optional] |
|**vatSum** | **Double** | Сумма НДС |  [optional] [readonly] |
|**sum** | **Double** | Сумма Приемки в копейках |  [optional] [readonly] |
|**payedSum** | **Double** | Сумма входящих платежей по Приемке |  [optional] [readonly] |
|**organization** | [**Organization**](Organization.md) |  |  [optional] |
|**organizationAccount** | [**Account**](Account.md) | Метаданные счета юрлица |  [optional] |
|**agent** | [**Agent**](Agent.md) | Метаданные контрагента |  [optional] |
|**agentAccount** | [**Account**](Account.md) | Метаданные счета контрагента |  [optional] |
|**store** | [**Store**](Store.md) | Метаданные склада |  [optional] |
|**state** | [**State**](State.md) | Метаданные статуса Приемки |  [optional] |
|**contract** | [**Contract**](Contract.md) | Метаданные договора |  [optional] |
|**project** | [**Project**](Project.md) | Метаданные проекта |  [optional] |
|**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива Файлов (максимальное количество файлов — 100) |  [optional] |
|**rate** | [**CurrencyRate**](CurrencyRate.md) |  |  [optional] |
|**overhead** | [**Overhead**](Overhead.md) |  |  [optional] |
|**positions** | [**SupplyPositionList**](SupplyPositionList.md) |  |  [optional] |
|**purchaseOrder** | [**PurchaseOrder**](PurchaseOrder.md) | Заказ поставщику, с которым связана Приемка  |  [optional] |
|**factureIn** | [**FactureIn**](FactureIn.md) | Счет-фактура полученный, с которым связана эта Приемка |  [optional] |
|**invoicesIn** | [**List&lt;InvoiceIn&gt;**](InvoiceIn.md) | Массив ссылок на связанные счета поставщиков |  [optional] |
|**payments** | [**List&lt;SupplyPaymentsInner&gt;**](SupplyPaymentsInner.md) | Массив ссылок на связанные платежи |  [optional] |
|**productionTask** | [**ProductionTask**](ProductionTask.md) | Связанное производственное задание |  [optional] |
|**returns** | [**List&lt;SupplyReturnsInner&gt;**](SupplyReturnsInner.md) | Массив ссылок на связанные возвраты  |  [optional] |
|**linkedSum** | **Double** | Сумма, оплаченная по данному документу |  |



