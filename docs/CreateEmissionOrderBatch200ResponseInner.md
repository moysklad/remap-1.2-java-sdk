

# CreateEmissionOrderBatch200ResponseInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Заказа кодов маркировки |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**created** | **String** | Момент создания Заказа кодов маркировки |  [optional] [readonly] |
|**description** | **String** | Комментарий |  [optional] |
|**documentState** | **String** | Состояние документов маркировки. Известные значения описаны в EmissionOrderDocumentState |  [optional] [readonly] |
|**emissionType** | **String** | Способ ввода в оборот. Известные значения описаны в EmissionOrderEmissionType |  [optional] |
|**externalCode** | **String** | Внешний код Заказа кодов маркировки |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**moment** | **String** | Дата документа |  [optional] |
|**name** | **String** | Наименование Заказа кодов маркировки |  [optional] |
|**organization** | [**Organization**](Organization.md) |  |  [optional] |
|**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) |  [optional] |
|**positions** | [**EmissionOrderPositionList**](EmissionOrderPositionList.md) |  |  [optional] |
|**printed** | **Boolean** | Напечатан ли документ |  [optional] [readonly] |
|**productionTasks** | [**List&lt;ProductionTask&gt;**](ProductionTask.md) | Массив ссылок на связанные производственные задания |  [optional] |
|**published** | **Boolean** | Опубликован ли документ |  [optional] [readonly] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**state** | [**State**](State.md) | Метаданные статуса Заказа кодов маркировки |  [optional] |
|**trackingType** | **String** | Тип маркируемой продукции. Известные значения описаны в TrackingType |  [optional] |
|**updated** | **String** | Момент последнего обновления |  [optional] [readonly] |
|**errors** | [**List&lt;ErrorErrorsInner&gt;**](ErrorErrorsInner.md) |  |  |



