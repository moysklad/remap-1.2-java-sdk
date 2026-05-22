

# ProductFolder

Группа товаров

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID группы товаров |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**name** | **String** | Наименование группы товаров |  [optional] |
|**code** | **String** | Код группы товаров |  [optional] |
|**externalCode** | **String** | Внешний код группы товаров |  [optional] |
|**archived** | **Boolean** | Добавлена ли группа товаров в архив |  [optional] |
|**pathName** | **String** | Наименование родительской группы |  [optional] [readonly] |
|**description** | **String** | Описание группы товаров |  [optional] |
|**vat** | **Integer** | НДС % |  [optional] |
|**vatEnabled** | **Boolean** | Включен ли НДС для группы |  [optional] |
|**effectiveVat** | **Integer** | Реальный НДС % |  [optional] [readonly] |
|**effectiveVatEnabled** | **Boolean** | Дополнительный признак для определения разграничения реального НДС |  [optional] [readonly] |
|**useParentVat** | **Boolean** | Используется ли ставка НДС родительской группы |  [optional] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**owner** | [**Employee**](Employee.md) | Владелец группы товаров. Может быть Meta объектом или полным объектом в зависимости от expand параметра |  [optional] |
|**updated** | **String** | Момент последнего обновления |  [optional] [readonly] |
|**productFolder** | [**ProductFolder**](ProductFolder.md) | Родительская группа товаров |  [optional] |
|**taxSystem** | **String** | Код системы налогообложения. Известные значения описаны в TaxSystem |  [optional] |



