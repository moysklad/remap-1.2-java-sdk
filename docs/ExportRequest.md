

# ExportRequest

Запрос на печать

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**template** | [**EmbeddedTemplate**](EmbeddedTemplate.md) |  |  [optional] |
|**extension** | [**ExtensionEnum**](#ExtensionEnum) | Расширение, в котором нужно напечатать форму. Допустимые значения: xls, pdf, html, ods.  |  [optional] |
|**templates** | [**List&lt;TemplateComposition&gt;**](TemplateComposition.md) | Набор шаблонов для печати комплекта документов. При использовании templates поле extension указывать не нужно.  |  [optional] |



## Enum: ExtensionEnum

| Name | Value |
|---- | -----|
| XLS | &quot;xls&quot; |
| PDF | &quot;pdf&quot; |
| HTML | &quot;html&quot; |
| ODS | &quot;ods&quot; |



