

# Store

Склад

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Склада |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) |  [optional] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**updated** | **String** | Момент последнего обновления |  [optional] [readonly] |
|**name** | **String** | Наименование Склада |  [optional] |
|**description** | **String** | Комментарий к Складу |  [optional] |
|**code** | **String** | Код Склада |  [optional] |
|**externalCode** | **String** | Внешний код Склада |  [optional] |
|**archived** | **Boolean** | Добавлен ли в архив |  [optional] |
|**address** | **String** | Адрес склада |  [optional] |
|**addressFull** | [**Address**](Address.md) | Адрес с детализацией |  [optional] |
|**pathName** | **String** | Группа Склада |  [optional] [readonly] |
|**parent** | [**Store**](Store.md) | Метаданные родительского склада (Группы) |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Дополнительные поля |  [optional] |
|**zones** | [**StoreZoneList**](StoreZoneList.md) | Зоны склада |  [optional] |
|**slots** | [**StoreSlotList**](StoreSlotList.md) | Ячейки склада |  [optional] |



