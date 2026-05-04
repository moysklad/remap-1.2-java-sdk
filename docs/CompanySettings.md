

# CompanySettings

Настройки компании (companysettings)

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**currency** | [**Currency**](Currency.md) |  |  [optional] |
|**priceTypes** | [**List&lt;PriceType&gt;**](PriceType.md) | Коллекция всех существующих типов цен |  [optional] |
|**discountStrategy** | **String** | Совместное применение скидок. Известные значения описаны в DiscountStrategy |  [optional] |
|**globalOperationNumbering** | **Boolean** | Использовать сквозную нумерацию документов |  [optional] |
|**checkShippingStock** | **Boolean** | Запретить отгрузку отсутствующих товаров |  [optional] |
|**checkMinPrice** | **Boolean** | Автоматически устанавливать минимальную цену |  [optional] |
|**useRecycleBin** | **Boolean** | Использовать корзину |  [optional] |
|**useCompanyAddress** | **Boolean** | Использовать адрес компании для электронных писем |  [optional] |
|**companyAddress** | **String** | Адрес компании для электронных писем |  [optional] |
|**accountCountry** | **String** | Страновая конфигурация аккаунта |  [optional] [readonly] |



