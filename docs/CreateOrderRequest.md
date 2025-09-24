# Dora.CreateOrderRequest

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**quantity** | **String** |  | 
**inverseLeverage** | **String** |  | 
**price** | **String** |  | [optional] 
**kind** | [**OrderKind**](OrderKind.md) |  | 
**side** | [**Side**](Side.md) |  | 
**positionId** | **String** | position ID to use for the order. required. | 
**orderBookId** | **String** | Required: the order book to submit the order to | 
**orderModifiers** | [**[OrderModifierKind]**](OrderModifierKind.md) |  | [optional] 
