

# CreateBonusTransaction200Response


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID бонусной операции |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**owner** | [**Employee**](Employee.md) |  |  [optional] |
|**agent** | [**Counterparty**](Counterparty.md) |  |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**organization** | [**Organization**](Organization.md) |  |  [optional] |
|**parentDocument** | [**Meta**](Meta.md) | Метаданные связанного документа бонусной операции |  [optional] |
|**applicable** | **Boolean** | Отметка о проведении |  [optional] |
|**bonusProgram** | [**BonusProgram**](BonusProgram.md) |  |  [optional] |
|**bonusValue** | **Integer** | Количество бонусных баллов |  [optional] |
|**transactionType** | [**TransactionTypeEnum**](#TransactionTypeEnum) | Тип бонусной операции |  [optional] |
|**transactionStatus** | [**TransactionStatusEnum**](#TransactionStatusEnum) | Статус бонусной операции |  [optional] [readonly] |
|**categoryType** | [**CategoryTypeEnum**](#CategoryTypeEnum) | Категория бонусной операции |  [optional] [readonly] |
|**code** | **String** | Код бонусной операции |  [optional] |
|**name** | **String** | Наименование бонусной операции |  [optional] |
|**externalCode** | **String** | Внешний код бонусной операции |  [optional] |
|**description** | **String** | Комментарий к бонусной операции |  [optional] |
|**moment** | **String** | Время проведения бонусной операции |  [optional] |
|**created** | **String** | Момент создания бонусной операции |  [optional] [readonly] |
|**updated** | **String** | Момент последнего обновления бонусной операции |  [optional] [readonly] |
|**executionDate** | **String** | Дата начисления бонусной операции |  [optional] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**updatedBy** | **String** | Автор последнего обновления (uid, используется для фильтрации) |  [optional] |



## Enum: TransactionTypeEnum

| Name | Value |
|---- | -----|
| EARNING | &quot;EARNING&quot; |
| SPENDING | &quot;SPENDING&quot; |



## Enum: TransactionStatusEnum

| Name | Value |
|---- | -----|
| WAIT_PROCESSING | &quot;WAIT_PROCESSING&quot; |
| COMPLETED | &quot;COMPLETED&quot; |
| CANCELED | &quot;CANCELED&quot; |



## Enum: CategoryTypeEnum

| Name | Value |
|---- | -----|
| REGULAR | &quot;REGULAR&quot; |
| WELCOME | &quot;WELCOME&quot; |



