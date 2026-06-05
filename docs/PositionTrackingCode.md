

# PositionTrackingCode

Код маркировки товара или транспортной упаковки в позиции Отгрузки

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**cis** | **String** | Значение кода маркировки |  [optional] |
|**type** | **String** | Тип кода маркировки. Известные значения описаны в PositionTrackingCodeType |  [optional] |
|**trackingCodes** | [**List&lt;PositionTrackingCode&gt;**](PositionTrackingCode.md) | Вложенные коды маркировки. Может присутствовать только если type имеет значения &#x60;consumerpack&#x60; или &#x60;transportpack&#x60;. Допустима вложенность кодов маркировки товаров в транспортные упаковки; транспортные упаковки не могут иметь вложенных упаковок.  |  [optional] |



