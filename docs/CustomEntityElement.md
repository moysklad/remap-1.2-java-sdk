

# CustomEntityElement

Элемент пользовательского справочника (customentity)

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID элемента пользовательского справочника |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**updated** | **String** | Момент последнего обновления элемента |  [optional] [readonly] |
|**name** | **String** | Наименование элемента пользовательского справочника |  [optional] |
|**code** | **String** | Код элемента пользовательского справочника |  [optional] |
|**description** | **String** | Описание элемента пользовательского справочника |  [optional] |
|**externalCode** | **String** | Внешний код элемента пользовательского справочника |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**owner** | [**Employee**](Employee.md) |  |  [optional] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |



