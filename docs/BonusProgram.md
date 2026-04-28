

# BonusProgram

Бонусная программа

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**earnRateRoublesToPoint** | **Integer** | Курс начисления |  [optional] |
|**earnWhileRedeeming** | **Boolean** | Разрешить одновременное начисление и списание бонусов |  [optional] |
|**postponedBonusesDelayDays** | **Integer** | Баллы начисляются через N дней |  [optional] |
|**spendRatePointsToRouble** | **Integer** | Курс списания |  [optional] |
|**welcomeBonusesEnabled** | **Boolean** | Возможность начисления приветственных баллов |  [optional] |
|**welcomeBonusesValue** | **Integer** | Количество приветственных баллов, начисляемых участникам бонусной программы |  [optional] |
|**welcomeBonusesMode** | [**WelcomeBonusesModeEnum**](#WelcomeBonusesModeEnum) | Условие начисления приветственных баллов |  [optional] |
|**maxPaidRatePercents** | **Integer** | Максимальный процент оплаты баллами |  [optional] |
|**allProducts** | **Boolean** | Для всех ли товаров скидка |  [optional] |
|**id** | **UUID** | ID дополнительного поля |  [optional] [readonly] |
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**name** | **String** | Наименование товара |  [optional] |
|**active** | **Boolean** | Включена ли скидка |  [optional] |
|**allAgents** | **Boolean** | Для всех ли агентов скидка |  [optional] |
|**agentTags** | **List&lt;String&gt;** | Тэги агентов |  [optional] |



## Enum: WelcomeBonusesModeEnum

| Name | Value |
|---- | -----|
| REGISTRATION | &quot;REGISTRATION&quot; |
| FIRST_PURCHASE | &quot;FIRST_PURCHASE&quot; |



