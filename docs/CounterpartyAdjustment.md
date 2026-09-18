

# CounterpartyAdjustment

Корректировка взаиморасчетов

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Корректировки взаиморасчетов |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**agent** | [**Agent**](Agent.md) | Метаданные контрагента или сотрудника |  [optional] |
|**applicable** | **Boolean** | Отметка о проведении |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**created** | **String** | Дата создания |  [optional] [readonly] |
|**deleted** | **String** | Момент последнего удаления Корректировки взаиморасчетов |  [optional] [readonly] |
|**description** | **String** | Комментарий Корректировки взаиморасчетов |  [optional] |
|**externalCode** | **String** | Внешний код Корректировки взаиморасчетов |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива Файлов (максимум 100) |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**moment** | **String** | Дата документа |  [optional] |
|**name** | **String** | Наименование Корректировки взаиморасчетов |  [optional] |
|**organization** | [**Organization**](Organization.md) |  |  [optional] |
|**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) |  [optional] |
|**printed** | **Boolean** | Напечатан ли документ |  [optional] [readonly] |
|**published** | **Boolean** | Опубликован ли документ |  [optional] [readonly] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**sum** | **Double** | Сумма Корректировки взаиморасчетов в копейках |  [optional] |
|**updated** | **String** | Момент последнего обновления Корректировки взаиморасчетов |  [optional] [readonly] |



