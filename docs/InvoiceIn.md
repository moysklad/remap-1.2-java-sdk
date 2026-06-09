

# InvoiceIn

Счет поставщика

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Счета поставщика |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**name** | **String** | Наименование Счета поставщика |  [optional] |
|**code** | **String** | Код Счета поставщика |  [optional] |
|**externalCode** | **String** | Внешний код Счета поставщика |  [optional] |
|**syncId** | **UUID** | ID синхронизации |  [optional] |
|**description** | **String** | Комментарий Счета поставщика |  [optional] |
|**created** | **String** | Дата создания |  [optional] [readonly] |
|**deleted** | **String** | Момент последнего удаления Счета поставщика |  [optional] [readonly] |
|**updated** | **String** | Момент последнего обновления Счета поставщика |  [optional] [readonly] |
|**moment** | **String** | Дата документа |  [optional] |
|**paymentPlannedMoment** | **String** | Планируемая дата оплаты |  [optional] |
|**incomingDate** | **String** | Входящая дата |  [optional] |
|**incomingNumber** | **String** | Входящий номер |  [optional] |
|**applicable** | **Boolean** | Отметка о проведении |  [optional] |
|**printed** | **Boolean** | Напечатан ли документ |  [optional] [readonly] |
|**published** | **Boolean** | Опубликован ли документ |  [optional] [readonly] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**vatEnabled** | **Boolean** | Учитывается ли НДС |  [optional] |
|**vatIncluded** | **Boolean** | Включен ли НДС в цену |  [optional] |
|**vatSum** | **Double** | Сумма НДС |  [optional] [readonly] |
|**sum** | **Double** | Сумма Счета в установленной валюте |  [optional] [readonly] |
|**payedSum** | **Double** | Сумма входящих платежей по Счету поставщика |  [optional] [readonly] |
|**shippedSum** | **Double** | Сумма отгруженного |  [optional] [readonly] |
|**organization** | [**Organization**](Organization.md) |  |  [optional] |
|**organizationAccount** | [**Account**](Account.md) | Метаданные счета юрлица |  [optional] |
|**agent** | [**Agent**](Agent.md) | Метаданные контрагента |  [optional] |
|**agentAccount** | [**Account**](Account.md) | Метаданные счета контрагента |  [optional] |
|**store** | [**Store**](Store.md) | Метаданные склада |  [optional] |
|**state** | [**State**](State.md) | Метаданные статуса счета |  [optional] |
|**contract** | [**Contract**](Contract.md) | Метаданные договора |  [optional] |
|**project** | [**Project**](Project.md) | Метаданные проекта |  [optional] |
|**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива Файлов |  [optional] |
|**rate** | [**CurrencyRate**](CurrencyRate.md) |  |  [optional] |
|**positions** | [**InvoiceInPositionList**](InvoiceInPositionList.md) |  |  [optional] |
|**purchaseOrder** | [**PurchaseOrder**](PurchaseOrder.md) | Заказ поставщику, с которым связан Счет поставщика |  [optional] |
|**supplies** | [**List&lt;Supply&gt;**](Supply.md) | Массив ссылок на связанные приемки |  [optional] |
|**payments** | [**List&lt;SalesReturnPaymentsInner&gt;**](SalesReturnPaymentsInner.md) | Массив ссылок на связанные операции |  [optional] |



