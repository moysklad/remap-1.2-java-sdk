

# CashInOperationAnyOf1

Возврат поставщику + linkedSum

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID возврата поставщику |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**name** | **String** | Наименование Возврата поставщику |  [optional] |
|**code** | **String** | Код Возврата поставщику |  [optional] |
|**externalCode** | **String** | Внешний код Возврата поставщику |  [optional] |
|**syncId** | **UUID** | ID синхронизации |  [optional] |
|**description** | **String** | Комментарий Возврата поставщику |  [optional] |
|**created** | **String** | Дата создания |  [optional] [readonly] |
|**deleted** | **String** | Момент последнего удаления Возврата поставщику |  [optional] [readonly] |
|**updated** | **String** | Момент последнего обновления Возврата поставщику |  [optional] [readonly] |
|**moment** | **String** | Дата документа |  [optional] |
|**applicable** | **Boolean** | Отметка о проведении |  [optional] |
|**printed** | **Boolean** | Напечатан ли документ |  [optional] [readonly] |
|**published** | **Boolean** | Опубликован ли документ |  [optional] [readonly] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**vatEnabled** | **Boolean** | Учитывается ли НДС |  [optional] |
|**vatIncluded** | **Boolean** | Включен ли НДС в цену |  [optional] |
|**vatSum** | **Double** | Сумма НДС |  [optional] [readonly] |
|**sum** | **Double** | Сумма Возврата поставщику в копейках |  [optional] [readonly] |
|**payedSum** | **Double** | Сумма входящих платежей по Возврату поставщику |  [optional] [readonly] |
|**organization** | [**Organization**](Organization.md) |  |  [optional] |
|**organizationAccount** | [**Account**](Account.md) | Метаданные счета юрлица |  [optional] |
|**agent** | [**Agent**](Agent.md) | Метаданные контрагента или юрлица |  [optional] |
|**agentAccount** | [**Account**](Account.md) | Метаданные счета контрагента |  [optional] |
|**store** | [**Store**](Store.md) |  |  [optional] |
|**state** | [**State**](State.md) | Метаданные статуса Возврата поставщику |  [optional] |
|**contract** | [**Contract**](Contract.md) | Метаданные договора |  [optional] |
|**project** | [**Project**](Project.md) | Метаданные проекта |  [optional] |
|**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива Файлов |  [optional] |
|**rate** | **CurrencyRate** |  |  [optional] |
|**positions** | [**PurchaseReturnPositionList**](PurchaseReturnPositionList.md) | Позиции Возврата поставщику |  [optional] |
|**supply** | [**Supply**](Supply.md) | Приемка, по которой произошел возврат |  [optional] |
|**factureOut** | [**FactureOut**](FactureOut.md) | Счет-фактура выданный, с которым связан этот возврат |  [optional] |
|**factureIn** | [**FactureIn**](FactureIn.md) | Счет-фактура полученный, с которым связан этот возврат |  [optional] |
|**payments** | [**List&lt;CustomerOrderPaymentsInner&gt;**](CustomerOrderPaymentsInner.md) | Массив ссылок на связанные платежи |  [optional] |
|**linkedSum** | **Double** | Сумма, оплаченная по данному документу |  |



