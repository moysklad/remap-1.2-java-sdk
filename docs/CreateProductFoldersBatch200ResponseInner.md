

# CreateProductFoldersBatch200ResponseInner


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
|**taxSystem** | [**TaxSystemEnum**](#TaxSystemEnum) | Код системы налогообложения |  [optional] |
|**errors** | [**List&lt;ErrorErrorsInner&gt;**](ErrorErrorsInner.md) |  |  |



## Enum: TaxSystemEnum

| Name | Value |
|---- | -----|
| GENERAL_TAX_SYSTEM | &quot;GENERAL_TAX_SYSTEM&quot; |
| SIMPLIFIED_TAX_SYSTEM_INCOME | &quot;SIMPLIFIED_TAX_SYSTEM_INCOME&quot; |
| SIMPLIFIED_TAX_SYSTEM_INCOME_OUTCOME | &quot;SIMPLIFIED_TAX_SYSTEM_INCOME_OUTCOME&quot; |
| UNIFIED_AGRICULTURAL_TAX | &quot;UNIFIED_AGRICULTURAL_TAX&quot; |
| PRESUMPTIVE_TAX_SYSTEM | &quot;PRESUMPTIVE_TAX_SYSTEM&quot; |
| PATENT_BASED | &quot;PATENT_BASED&quot; |
| TAX_SYSTEM_SAME_AS_GROUP | &quot;TAX_SYSTEM_SAME_AS_GROUP&quot; |



