

# CreateTasksBatch200ResponseInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Задачи |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**agent** | [**Agent**](Agent.md) | Метаданные Контрагента или юрлица, связанного с задачей |  [optional] |
|**assignee** | [**Employee**](Employee.md) |  |  [optional] |
|**author** | [**Employee**](Employee.md) |  |  [optional] |
|**authorApplication** | [**Application**](Application.md) |  |  [optional] |
|**completed** | **String** | Время выполнения задачи |  [optional] [readonly] |
|**created** | **String** | Момент создания |  [optional] [readonly] |
|**description** | **String** | Текст задачи |  [optional] |
|**done** | **Boolean** | Отметка о выполнении задачи |  [optional] |
|**dueToDate** | **String** | Срок задачи |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива Файлов |  [optional] |
|**implementer** | [**Employee**](Employee.md) |  |  [optional] |
|**notes** | [**TaskNotes**](TaskNotes.md) |  |  [optional] |
|**operation** | [**DocumentMetadata**](DocumentMetadata.md) |  |  [optional] |
|**state** | [**State**](State.md) | Метаданные типа задачи |  [optional] |
|**updated** | **String** | Момент последнего обновления Задачи |  [optional] [readonly] |
|**errors** | [**List&lt;ErrorErrorsInner&gt;**](ErrorErrorsInner.md) |  |  |



