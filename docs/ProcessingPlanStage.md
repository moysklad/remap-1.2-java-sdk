

# ProcessingPlanStage

Этап Техкарты

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID этапа Техкарты |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**enableHourAccounting** | **Boolean** | Признак активности учета по нормо-часам |  [optional] |
|**cost** | **Double** | Стоимость производства на определенном этапе |  [optional] |
|**labourCost** | **Double** | Оплата труда на определенном этапе |  [optional] |
|**standardHour** | **Double** | Нормо-часы на определенном этапе |  [optional] |
|**standardHourCost** | **Double** | Стоимость нормо-часа |  [optional] [readonly] |
|**processingProcessPosition** | [**ProcessingProcessPosition**](ProcessingProcessPosition.md) |  |  [optional] |



