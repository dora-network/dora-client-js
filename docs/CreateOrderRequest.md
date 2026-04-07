# Dora.CreateOrderRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**quantity** | **String** |  | 
**inverseLeverage** | **String** |  | 
**price** | **String** |  | [optional] 
**kind** | [**OrderKind**](OrderKind.md) |  | 
**side** | [**Side**](Side.md) | Required: Must be either &#39;BUY&#39; or &#39;SELL&#39; | 
**fromGlobalPosition** | **Boolean** | use global position for the order or isolated. required. | 
**orderBookId** | **String** | Required: the order book to submit the order to | 
**orderModifiers** | [**[OrderModifierKind]**](OrderModifierKind.md) |  | [optional] 
**goodTillDate** | **Date** |  | [optional] 
**clientOrderId** | **String** | An optional client-provided identifier for the order. | [optional] 
**stopLossPrice** | **String** | Stop loss price | [optional] 
**takeProfitPrice** | **String** | Take profit price | [optional] 


