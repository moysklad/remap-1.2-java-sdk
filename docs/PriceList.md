

# PriceList

Прайс-лист

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Прайс-листа |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**applicable** | **Boolean** | Отметка о проведении |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**code** | **String** | Код Прайс-листа |  [optional] |
|**columns** | [**List&lt;PriceListColumn&gt;**](PriceListColumn.md) | Массив столбцов описания таблицы |  [optional] |
|**created** | **String** | Дата создания |  [optional] [readonly] |
|**deleted** | **String** | Момент последнего удаления Прайс-листа |  [optional] [readonly] |
|**description** | **String** | Комментарий Прайс-листа |  [optional] |
|**externalCode** | **String** | Внешний код Прайс-листа |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива Файлов |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**moment** | **String** | Дата документа |  [optional] |
|**name** | **String** | Наименование Прайс-листа |  [optional] |
|**organization** | [**Organization**](Organization.md) |  |  [optional] |
|**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) |  [optional] |
|**positions** | [**PriceListPositionList**](PriceListPositionList.md) | Метаданные позиций Прайс-листа |  [optional] |
|**priceType** | [**PriceType**](PriceType.md) | Объект типа цены |  [optional] |
|**printed** | **Boolean** | Напечатан ли документ |  [optional] [readonly] |
|**published** | **Boolean** | Опубликован ли документ |  [optional] [readonly] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**state** | [**State**](State.md) | Метаданные статуса Прайс-листа |  [optional] |
|**syncId** | **UUID** | ID синхронизации. После заполнения недоступен для изменения |  [optional] |
|**updated** | **String** | Момент последнего обновления Прайс-листа |  [optional] [readonly] |



