

# Processing

Техоперация

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID техоперации |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**name** | **String** | Наименование техоперации |  [optional] |
|**code** | **String** | Код техоперации |  [optional] |
|**externalCode** | **String** | Внешний код техоперации |  [optional] |
|**syncId** | **UUID** | ID синхронизации |  [optional] |
|**description** | **String** | Комментарий техоперации |  [optional] |
|**created** | **String** | Дата создания |  [optional] [readonly] |
|**deleted** | **String** | Момент последнего удаления техоперации |  [optional] [readonly] |
|**updated** | **String** | Момент последнего обновления техоперации |  [optional] [readonly] |
|**moment** | **String** | Дата документа |  [optional] |
|**applicable** | **Boolean** | Отметка о проведении |  [optional] |
|**printed** | **Boolean** | Напечатан ли документ |  [optional] [readonly] |
|**published** | **Boolean** | Опубликован ли документ |  [optional] [readonly] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**organization** | [**Organization**](Organization.md) |  |  [optional] |
|**organizationAccount** | [**Account**](Account.md) | Метаданные счета юрлица |  [optional] |
|**processingPlan** | [**ProcessingPlan**](ProcessingPlan.md) | Метаданные техкарты |  [optional] |
|**processingOrder** | [**ProcessingOrder**](ProcessingOrder.md) | Метаданные заказа на производство |  [optional] |
|**project** | [**Project**](Project.md) | Метаданные проекта |  [optional] |
|**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**state** | [**State**](State.md) | Метаданные статуса техоперации |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива файлов |  [optional] |
|**productsStore** | [**Store**](Store.md) |  |  [optional] |
|**materialsStore** | [**Store**](Store.md) |  |  [optional] |
|**products** | [**ProcessingProductList**](ProcessingProductList.md) |  |  [optional] |
|**materials** | [**ProcessingMaterialList**](ProcessingMaterialList.md) |  |  [optional] |
|**quantity** | **Double** | Объем производства |  [optional] |
|**processingSum** | **Double** | Затраты на производство за единицу объема производства |  [optional] |



