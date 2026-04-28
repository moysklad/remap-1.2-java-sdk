

# Service


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID услуги |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**archived** | **Boolean** | Добавлена ли услуга в архив |  [optional] |
|**name** | **String** | Наименование услуги |  [optional] |
|**code** | **String** | Код услуги |  [optional] |
|**externalCode** | **String** | Внешний код услуги |  [optional] |
|**pathName** | **String** | Наименование группы, в которую входит услуга |  [optional] [readonly] |
|**description** | **String** | Описание услуги |  [optional] |
|**vat** | **Integer** | НДС % |  [optional] |
|**vatEnabled** | **Boolean** | Включен ли НДС для услуги |  [optional] |
|**useParentVat** | **Boolean** | Используется ли ставка НДС родительской группы |  [optional] |
|**effectiveVat** | **Integer** | Реальный НДС % |  [optional] [readonly] |
|**effectiveVatEnabled** | **Boolean** | Дополнительный признак для определения разграничения реального НДС |  [optional] [readonly] |
|**discountProhibited** | **Boolean** | Признак запрета скидок |  [optional] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**owner** | [**Employee**](Employee.md) | Метаданные владельца (Сотрудника) |  [optional] |
|**updated** | **String** | Момент последнего обновления сущности |  [optional] [readonly] |
|**buyPrice** | [**BuyPrice**](BuyPrice.md) |  |  [optional] |
|**salePrices** | [**List&lt;SalePrice&gt;**](SalePrice.md) | Цены продажи |  [optional] |
|**uom** | [**Uom**](Uom.md) | Метаданные единиц измерения |  [optional] |
|**productFolder** | [**ProductFolder**](ProductFolder.md) | Метаданные группы Услуги |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива Файлов |  [optional] |
|**barcodes** | [**List&lt;Barcode&gt;**](Barcode.md) | Штрихкоды услуги |  [optional] |
|**paymentItemType** | [**PaymentItemTypeEnum**](#PaymentItemTypeEnum) | Признак предмета расчета |  [optional] |
|**taxSystem** | [**TaxSystemEnum**](#TaxSystemEnum) | Код системы налогообложения |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Дополнительные поля |  [optional] |
|**minPrice** | [**MinPrice**](MinPrice.md) |  |  [optional] |
|**syncId** | **UUID** | ID синхронизации |  [optional] |



## Enum: PaymentItemTypeEnum

| Name | Value |
|---- | -----|
| WORK | &quot;WORK&quot; |
| SERVICE | &quot;SERVICE&quot; |
| COMPOUND_PAYMENT_ITEM | &quot;COMPOUND_PAYMENT_ITEM&quot; |
| PROVIDING_RID | &quot;PROVIDING_RID&quot; |
| ANOTHER_PAYMENT_ITEM | &quot;ANOTHER_PAYMENT_ITEM&quot; |



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



