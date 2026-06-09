

# FactureIn

Счет-фактура полученный (facturein)

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Счета-фактуры полученного |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**agent** | [**Agent**](Agent.md) | Метаданные контрагента или юрлица |  [optional] |
|**applicable** | **Boolean** | Отметка о проведении |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**code** | **String** | Код Счета-фактуры полученного |  [optional] |
|**contract** | [**Contract**](Contract.md) | Метаданные договора |  [optional] |
|**created** | **String** | Дата создания |  [optional] [readonly] |
|**deleted** | **String** | Момент последнего удаления Счета-фактуры полученного |  [optional] [readonly] |
|**description** | **String** | Комментарий Счета-фактуры полученного |  [optional] |
|**externalCode** | **String** | Внешний код Счета-фактуры полученного |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива файлов |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**moment** | **String** | Дата документа |  [optional] |
|**name** | **String** | Наименование Счета-фактуры полученного |  [optional] |
|**organization** | [**Organization**](Organization.md) |  |  [optional] |
|**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) |  [optional] |
|**printed** | **Boolean** | Напечатан ли документ |  [optional] [readonly] |
|**published** | **Boolean** | Опубликован ли документ |  [optional] [readonly] |
|**rate** | **CurrencyRate** | Валюта документа. Если значение курса валюты не указано, используется курс из справочника валют.  |  [optional] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**state** | [**State**](State.md) | Метаданные статуса Счета-фактуры полученного |  [optional] |
|**sum** | **Double** | Сумма Счета-фактуры полученного в установленной валюте |  [optional] [readonly] |
|**syncId** | **UUID** | ID синхронизации |  [optional] |
|**updated** | **String** | Момент последнего обновления Счета-фактуры полученного |  [optional] [readonly] |
|**supplies** | [**List&lt;Supply&gt;**](Supply.md) | Массив ссылок на связанные приемки |  [optional] |
|**payments** | [**List&lt;PaymentOut&gt;**](PaymentOut.md) | Массив ссылок на связанные исходящие платежи |  [optional] |
|**incomingNumber** | **String** | Входящий номер |  [optional] |
|**incomingDate** | **String** | Входящая дата |  [optional] |



