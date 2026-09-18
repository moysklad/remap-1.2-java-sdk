

# Permissions

Права на сущность. BASE включает view, create, update и delete; DICTIONARY дополнительно включает print; OPERATION — print и approve. Для GTINList используются view, create и delete, для trackingCodeList — view и print. Известные значения описаны в PermissionValue. Область действия расширяется по цепочкам NO → OWN → OWN_SHARED → OWN_GROUP_SHARED → ALL и NO → OWN → OWN_GROUP → OWN_GROUP_SHARED → ALL. Неуказанное действие запрещено сотруднику. 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**view** | **String** | Смотреть. Известные значения описаны в PermissionValue. |  [optional] |
|**print** | **String** | Печатать. Известные значения описаны в PermissionValue. Значение совпадает с view или отсутствует. |  [optional] |
|**create** | **String** | Создавать. Известные значения описаны в PermissionValue. Значение совпадает с view или отсутствует. |  [optional] |
|**update** | **String** | Редактировать. Известные значения описаны в PermissionValue. Область действия не шире view; поле может отсутствовать. |  [optional] |
|**delete** | **String** | Удалять. Известные значения описаны в PermissionValue. Значение совпадает с update или отсутствует. |  [optional] |
|**approve** | **String** | Проводить. Известные значения описаны в PermissionValue. Значение совпадает с view или отсутствует. |  [optional] |



