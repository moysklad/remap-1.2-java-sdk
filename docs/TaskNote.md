

# TaskNote

Комментарий к Задаче

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID комментария к Задаче |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**author** | [**Employee**](Employee.md) |  |  [optional] |
|**authorApplication** | [**Application**](Application.md) |  |  [optional] |
|**moment** | **String** | Момент создания комментария |  [optional] [readonly] |
|**text** | **String** | Текст комментария |  [optional] |
|**files** | [**TaskNoteFileList**](TaskNoteFileList.md) | Метаданные массива Файлов |  [optional] |



