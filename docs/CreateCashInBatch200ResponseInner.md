

# CreateCashInBatch200ResponseInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Приходного ордера |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**applicable** | **Boolean** | Отметка о проведении |  [optional] |
|**name** | **String** | Наименование Приходного ордера |  [optional] |
|**code** | **String** | Код Приходного ордера |  [optional] |
|**externalCode** | **String** | Внешний код Приходного ордера |  [optional] |
|**syncId** | **UUID** | ID синхронизации |  [optional] |
|**description** | **String** | Комментарий Приходного ордера |  [optional] |
|**created** | **String** | Дата создания |  [optional] [readonly] |
|**deleted** | **String** | Момент последнего удаления Приходного ордера |  [optional] [readonly] |
|**updated** | **String** | Момент последнего обновления Приходного ордера |  [optional] [readonly] |
|**moment** | **String** | Дата документа |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**contract** | [**Contract**](Contract.md) | Метаданные договора |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива файлов |  [optional] |
|**paymentPurpose** | **String** | Основание |  [optional] |
|**printed** | **Boolean** | Напечатан ли документ |  [optional] [readonly] |
|**project** | [**Project**](Project.md) | Метаданные проекта |  [optional] |
|**published** | **Boolean** | Опубликован ли документ |  [optional] [readonly] |
|**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**salesChannel** | [**SalesChannel**](SalesChannel.md) | Метаданные канала продаж |  [optional] |
|**shared** | **Boolean** | Общий доступ |  [optional] [readonly] |
|**state** | [**State**](State.md) | Метаданные статуса Приходного ордера |  [optional] |
|**rate** | [**CurrencyRate**](CurrencyRate.md) |  |  [optional] |
|**organization** | [**Organization**](Organization.md) |  |  [optional] |
|**agent** | [**Counterparty**](Counterparty.md) |  |  [optional] |
|**sum** | **Double** | Сумма Приходного ордера в установленной валюте |  [optional] [readonly] |
|**vatSum** | **Double** | Сумма НДС |  [optional] [readonly] |
|**factureOut** | [**FactureOut**](FactureOut.md) | Счет-фактура выданный, с которым связан этот платеж |  [optional] |
|**operations** | [**List&lt;CashInOperation&gt;**](CashInOperation.md) | Связанные операции. Допустимые типы по &#x60;meta.type&#x60;: customerorder, purchasereturn, demand, invoiceout, commissionreportin, retailshift.  |  [optional] |
|**errors** | [**List&lt;ErrorErrorsInner&gt;**](ErrorErrorsInner.md) |  |  |



