

# CreateProcessingPlanBatch200ResponseInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Техкарты |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**archived** | **Boolean** | Добавлена ли Техкарта в архив |  [optional] |
|**code** | **String** | Код Техкарты |  [optional] |
|**cost** | **Double** | Стоимость производства |  [optional] |
|**costDistributionType** | **String** | Тип распределения себестоимости. Возможные значения описаны в CostDistributionType |  [optional] [readonly] |
|**externalCode** | **String** | Внешний код Техкарты |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**name** | **String** | Наименование Техкарты |  [optional] |
|**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) |  [optional] |
|**parent** | [**ProcessingPlanFolder**](ProcessingPlanFolder.md) |  |  [optional] |
|**pathName** | **String** | Наименование группы, в которую входит Техкарта |  [optional] [readonly] |
|**processingProcess** | [**ProcessingProcess**](ProcessingProcess.md) |  |  [optional] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**updated** | **String** | Момент последнего обновления Техкарты |  [optional] [readonly] |
|**stages** | [**ProcessingPlanStageList**](ProcessingPlanStageList.md) | Коллекция метаданных этапов Техкарты |  [optional] |
|**materials** | [**ProcessingPlanMaterialList**](ProcessingPlanMaterialList.md) | Коллекция метаданных материалов Техкарты |  [optional] |
|**products** | [**ProcessingPlanProductList**](ProcessingPlanProductList.md) | Коллекция метаданных готовых продуктов Техкарты |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**errors** | [**List&lt;ErrorErrorsInner&gt;**](ErrorErrorsInner.md) |  |  |



