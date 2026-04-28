

# CreateCurrenciesBatch200ResponseInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID валюты |  [optional] [readonly] |
|**system** | **Boolean** | Системная валюта |  [optional] [readonly] |
|**name** | **String** | Краткое наименование валюты |  [optional] |
|**fullName** | **String** | Полное наименование валюты |  [optional] |
|**code** | **String** | Цифровой код валюты |  [optional] |
|**isoCode** | **String** | Буквенный код валюты |  [optional] |
|**multiplicity** | **Integer** | Кратность курса валюты |  [optional] |
|**rate** | **Float** | Курс валюты |  [optional] |
|**margin** | **Float** | Наценка при автоматическом обновлении курса |  [optional] |
|**indirect** | **Boolean** | Признак обратного курса валюты |  [optional] |
|**rateUpdateType** | [**RateUpdateTypeEnum**](#RateUpdateTypeEnum) | Способ обновления курса валюты |  [optional] |
|**archived** | **Boolean** | Добавлена ли валюта в архив |  [optional] |
|**_default** | **Boolean** | Валюта учета по умолчанию |  [optional] |
|**majorUnit** | [**CurrencyMajorUnit**](CurrencyMajorUnit.md) |  |  [optional] |
|**minorUnit** | [**CurrencyMinorUnit**](CurrencyMinorUnit.md) |  |  [optional] |
|**errors** | [**List&lt;ErrorErrorsInner&gt;**](ErrorErrorsInner.md) |  |  |



## Enum: RateUpdateTypeEnum

| Name | Value |
|---- | -----|
| MANUAL | &quot;manual&quot; |
| AUTO | &quot;auto&quot; |



