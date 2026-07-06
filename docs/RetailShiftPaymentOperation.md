

# RetailShiftPaymentOperation

Элемент массива `paymentOperations` розничной смены.  Допустимые `meta.type`: cashin, paymentin. 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Входящего платежа |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**applicable** | **Boolean** | Отметка о проведении |  [optional] |
|**name** | **String** | Наименование Входящего платежа |  [optional] |
|**code** | **String** | Код Входящего платежа |  [optional] |
|**externalCode** | **String** | Внешний код Входящего платежа |  [optional] |
|**syncId** | **UUID** | ID синхронизации |  [optional] |
|**description** | **String** | Комментарий Входящего платежа |  [optional] |
|**created** | **String** | Дата создания |  [optional] [readonly] |
|**deleted** | **String** | Момент последнего удаления Входящего платежа |  [optional] [readonly] |
|**updated** | **String** | Момент последнего обновления Входящего платежа |  [optional] [readonly] |
|**moment** | **String** | Дата документа |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**contract** | [**Contract**](Contract.md) | Метаданные договора |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива файлов |  [optional] |
|**paymentPurpose** | **String** | Назначение платежа |  [optional] |
|**printed** | **Boolean** | Напечатан ли документ |  [optional] [readonly] |
|**project** | [**Project**](Project.md) | Метаданные проекта |  [optional] |
|**published** | **Boolean** | Опубликован ли документ |  [optional] [readonly] |
|**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**salesChannel** | [**SalesChannel**](SalesChannel.md) | Метаданные канала продаж |  [optional] |
|**shared** | **Boolean** | Общий доступ |  [optional] [readonly] |
|**state** | [**State**](State.md) | Метаданные статуса Входящего платежа |  [optional] |
|**rate** | [**CurrencyRate**](CurrencyRate.md) |  |  [optional] |
|**organization** | [**Organization**](Organization.md) |  |  [optional] |
|**agent** | [**Agent**](Agent.md) | Метаданные контрагента |  [optional] |
|**sum** | **Double** | Сумма Входящего платежа в установленной валюте |  [optional] [readonly] |
|**vatSum** | **Double** | Сумма НДС |  [optional] [readonly] |
|**factureOut** | [**FactureOut**](FactureOut.md) | Счет-фактура выданный, с которым связан этот платеж |  [optional] |
|**operations** | [**List&lt;FinanceInOperationAbstract&gt;**](FinanceInOperationAbstract.md) | Связанные операции. Допустимые типы по &#x60;meta.type&#x60;: customerorder, purchasereturn, demand, invoiceout, commissionreportin, retailshift.  |  [optional] |
|**linkedSum** | **Double** | Сумма, оплаченная по данному документу |  |
|**agentAccount** | [**Account**](Account.md) | Метаданные счета контрагента |  [optional] |
|**organizationAccount** | [**Account**](Account.md) | Метаданные счета юрлица |  [optional] |
|**incomingNumber** | **String** | Входящий номер |  [optional] |
|**incomingDate** | **String** | Входящая дата |  [optional] |



