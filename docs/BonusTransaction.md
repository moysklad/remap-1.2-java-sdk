

# BonusTransaction

Бонусная операция (bonustransaction)

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
|**parentDocument** | [**StabEntity**](StabEntity.md) |  |  [optional] |
|**applicable** | **Boolean** | Отметка о проведении |  [optional] |
|**bonusProgram** | [**BonusProgram**](BonusProgram.md) |  |  [optional] |
|**bonusValue** | **Integer** | Количество бонусных баллов |  [optional] |
|**transactionType** | **String** | Тип бонусной операции. Известные значения описаны в TransactionType |  [optional] |
|**transactionStatus** | **String** | Статус бонусной операции. Известные значения описаны в TransactionStatus |  [optional] [readonly] |
|**categoryType** | **String** | Категория бонусной операции. Известные значения описаны в CategoryType |  [optional] [readonly] |
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



