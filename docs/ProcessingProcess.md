

# ProcessingProcess

Техпроцесс

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Техпроцесса |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**owner** | [**Employee**](Employee.md) | Метаданные владельца (Сотрудника) |  [optional] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**updated** | **String** | Момент последнего обновления Техпроцесса |  [optional] [readonly] |
|**name** | **String** | Наименование Техпроцесса |  [optional] |
|**description** | **String** | Комментарий Техпроцесса |  [optional] |
|**externalCode** | **String** | Внешний код Техпроцесса |  [optional] |
|**archived** | **Boolean** | Добавлен ли Техпроцесс в архив |  [optional] |
|**positions** | [**ProcessingProcessPositionList**](ProcessingProcessPositionList.md) |  |  [optional] |



