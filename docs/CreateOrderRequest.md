# Dora.CreateOrderRequest

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**quantity** | **String** |  | [optional] 
**inverseLeverage** | **Number** | Required: Inverse leverage for the order, must be between 0 and 1 (inclusive) | [optional] 
**price** | **String** |  | [optional] 
**kind** | **String** |  | [optional] 
**side** | **String** | Required: Must be either &#x27;BUY&#x27; or &#x27;SELL&#x27; | [optional] 
**orderBookId** | **String** | Required: the order book to submit the order to | [optional] 
**userText** | **String** | Optional: User-defined text for the order, e.g., &#x27;buying dips&#x27; | [optional] 
**orderModifiers** | **[String]** |  | [optional] 

<a name="KindEnum"></a>
## Enum: KindEnum

* `MARKET` (value: `"MARKET"`)
* `LIMIT` (value: `"LIMIT"`)


<a name="[OrderModifiersEnum]"></a>
## Enum: [OrderModifiersEnum]

* `MAX_BUY` (value: `"MAX_BUY"`)

