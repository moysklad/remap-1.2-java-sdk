

# Inventory

Инвентаризация

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Инвентаризации |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**code** | **String** | Код Инвентаризации |  [optional] |
|**created** | **String** | Дата создания |  [optional] [readonly] |
|**deleted** | **String** | Момент последнего удаления Инвентаризации |  [optional] [readonly] |
|**description** | **String** | Комментарий Инвентаризации |  [optional] |
|**externalCode** | **String** | Внешний код Инвентаризации |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива Файлов (Максимальное количество файлов - 100) |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**moment** | **String** | Дата документа |  [optional] |
|**name** | **String** | Наименование Инвентаризации |  [optional] |
|**organization** | [**Organization**](Organization.md) |  |  [optional] |
|**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) |  [optional] |
|**positions** | [**InventoryPositionList**](InventoryPositionList.md) | Метаданные позиций Инвентаризации |  [optional] |
|**printed** | **Boolean** | Напечатан ли документ |  [optional] [readonly] |
|**published** | **Boolean** | Опубликован ли документ |  [optional] [readonly] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**state** | [**State**](State.md) | Метаданные статуса Инвентаризации |  [optional] |
|**store** | [**Store**](Store.md) |  |  [optional] |
|**sum** | **Double** | Сумма Инвентаризации в копейках |  [optional] [readonly] |
|**syncId** | **UUID** | ID синхронизации |  [optional] |
|**updated** | **String** | Момент последнего обновления Инвентаризации |  [optional] [readonly] |
|**enters** | [**List&lt;Enter&gt;**](Enter.md) | Связанные с Инвентаризацией оприходования |  [optional] |
|**losses** | [**List&lt;Loss&gt;**](Loss.md) | Связанные с Инвентаризацией списания |  [optional] |



