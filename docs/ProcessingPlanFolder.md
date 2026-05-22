

# ProcessingPlanFolder

Группа техкарт

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Группы техкарт |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**name** | **String** | Наименование Группы техкарт |  [optional] |
|**code** | **String** | Код Группы техкарт |  [optional] |
|**externalCode** | **String** | Внешний код Группы техкарт |  [optional] |
|**description** | **String** | Описание Группы техкарт |  [optional] |
|**archived** | **Boolean** | Добавлена ли Группа техкарт в архив |  [optional] |
|**pathName** | **String** | Наименование группы техкарт, в которую входит данная группа (иерархия) |  [optional] [readonly] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**updated** | **String** | Момент последнего обновления сущности |  [optional] [readonly] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**owner** | [**Employee**](Employee.md) | Метаданные владельца (сотрудника) |  [optional] |
|**processingplanfolder** | [**ProcessingPlanFolder**](ProcessingPlanFolder.md) | Родительская Группа техкарт. Для смены иерархии и поля pathName обновите эту ссылку |  [optional] |



