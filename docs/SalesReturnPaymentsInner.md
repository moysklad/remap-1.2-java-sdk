

# SalesReturnPaymentsInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Расходного ордера |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**name** | **String** | Наименование Расходного ордера |  [optional] |
|**code** | **String** | Код Расходного ордера |  [optional] |
|**externalCode** | **String** | Внешний код Расходного ордера |  [optional] |
|**syncId** | **UUID** | ID синхронизации |  [optional] |
|**description** | **String** | Комментарий Расходного ордера |  [optional] |
|**created** | **String** | Дата создания |  [optional] [readonly] |
|**deleted** | **String** | Момент последнего удаления Расходного ордера |  [optional] [readonly] |
|**updated** | **String** | Момент последнего обновления Расходного ордера |  [optional] [readonly] |
|**moment** | **String** | Дата документа |  [optional] |
|**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**applicable** | **Boolean** | Отметка о проведении |  [optional] |
|**printed** | **Boolean** | Напечатан ли документ |  [optional] [readonly] |
|**published** | **Boolean** | Опубликован ли документ |  [optional] [readonly] |
|**rate** | [**CurrencyRate**](CurrencyRate.md) |  |  [optional] |
|**organization** | [**Organization**](Organization.md) |  |  [optional] |
|**agent** | [**Agent**](Agent.md) | Метаданные контрагента или юрлица |  [optional] |
|**expenseItem** | [**ExpenseItem**](ExpenseItem.md) | Метаданные статьи расхода |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**contract** | [**Contract**](Contract.md) | Метаданные договора |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива файлов |  [optional] |
|**noClosingDocs** | **Boolean** | Признак \&quot;Без закрывающих документов\&quot; |  [optional] |
|**paymentPurpose** | **String** | Основание |  [optional] |
|**project** | [**Project**](Project.md) | Метаданные проекта |  [optional] |
|**salesChannel** | [**SalesChannel**](SalesChannel.md) | Метаданные канала продаж |  [optional] |
|**shared** | **Boolean** | Общий доступ |  [optional] [readonly] |
|**state** | [**State**](State.md) | Метаданные статуса Расходного ордера |  [optional] |
|**sum** | **Double** | Сумма расходного ордера в установленной валюте |  [optional] [readonly] |
|**vatSum** | **Double** | Сумма НДС |  [optional] [readonly] |
|**factureIn** | [**FactureIn**](FactureIn.md) | Счет-фактура полученный, с которым связан этот платеж |  [optional] |
|**agentAccount** | [**Account**](Account.md) | Метаданные счета контрагента или юрлица |  [optional] |
|**organizationAccount** | [**Account**](Account.md) | Метаданные счета юрлица |  [optional] |
|**operations** | [**List&lt;CashOutOperation&gt;**](CashOutOperation.md) | Связанные операции: полное тело документа плюс &#x60;linkedSum&#x60;. Допустимые типы по &#x60;meta.type&#x60;: salesreturn, supply, invoicein, purchaseorder, commissionreportout. См. &#x60;CashOutOperation&#x60;.  |  [optional] |



