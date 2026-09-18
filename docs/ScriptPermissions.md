

# ScriptPermissions

Права на задачи. NO для view и done допустимо, только если остальные права равны NO. Если view отличается от NO, поле done обязательно и должно совпадать с view. Известные значения описаны в ScriptPermissionValue. 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**view** | **String** | Смотреть. Допустимые значения — NO, AUTHOR_OR_ASSIGNEE, ALL. Известные значения описаны в ScriptPermissionValue. |  [optional] |
|**create** | **String** | Создавать. Допустимые значения — NO, ALL. Область действия не шире view; поле может отсутствовать. Известные значения описаны в ScriptPermissionValue. |  [optional] |
|**update** | **String** | Редактировать. Допустимые значения — NO, AUTHOR, AUTHOR_OR_ASSIGNEE, ALL. Область действия не шире view; поле может отсутствовать. Известные значения описаны в ScriptPermissionValue. |  [optional] |
|**delete** | **String** | Удалять. Допустимые значения — NO, AUTHOR, AUTHOR_OR_ASSIGNEE, ALL. Область действия не шире update; поле может отсутствовать. Известные значения описаны в ScriptPermissionValue. |  [optional] |
|**done** | **String** | Выполнять. Допустимые значения — NO, ASSIGNEE, AUTHOR_OR_ASSIGNEE, ALL. Область действия не шире view; при view, отличном от NO, обязательно и совпадает с view. Известные значения описаны в ScriptPermissionValue. |  [optional] |



