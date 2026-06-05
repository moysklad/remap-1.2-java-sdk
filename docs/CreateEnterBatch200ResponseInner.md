

# CreateEnterBatch200ResponseInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Оприходования |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**applicable** | **Boolean** | Отметка о проведении |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**code** | **String** | Код Оприходования |  [optional] |
|**created** | **String** | Дата создания |  [optional] [readonly] |
|**deleted** | **String** | Момент последнего удаления Оприходования |  [optional] [readonly] |
|**description** | **String** | Комментарий Оприходования |  [optional] |
|**externalCode** | **String** | Внешний код Оприходования |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива Файлов |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**moment** | **String** | Дата документа |  [optional] |
|**name** | **String** | Номер Оприходования |  [optional] |
|**organization** | [**Organization**](Organization.md) |  |  [optional] |
|**overhead** | [**Overhead**](Overhead.md) |  |  [optional] |
|**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) |  [optional] |
|**positions** | [**EnterPositionList**](EnterPositionList.md) | Метаданные позиций Оприходования |  [optional] |
|**printed** | **Boolean** | Напечатан ли документ |  [optional] [readonly] |
|**project** | [**Project**](Project.md) | Метаданные проекта |  [optional] |
|**published** | **Boolean** | Опубликован ли документ |  [optional] [readonly] |
|**rate** | **CurrencyRate** |  |  [optional] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**state** | [**State**](State.md) | Метаданные статуса Оприходования |  [optional] |
|**store** | [**Store**](Store.md) |  |  [optional] |
|**sum** | **Double** | Сумма Оприходования в копейках |  [optional] [readonly] |
|**syncId** | **UUID** | ID синхронизации |  [optional] |
|**updated** | **String** | Момент последнего обновления Оприходования |  [optional] [readonly] |
|**errors** | [**List&lt;ErrorErrorsInner&gt;**](ErrorErrorsInner.md) |  |  |



