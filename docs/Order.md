# Dora.Order

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**orderId** | **String** |  | [optional] 
**orderBookId** | **String** |  | [optional] 
**kind** | [**OrderKind**](OrderKind.md) |  | [optional] 
**originalPrice** | **String** | If Kind is LIMIT, this is the original limit price. If Kind is MARKET, this may be 0 or omitted. | [optional] 
**avgFillPrice** | **String** |  | [optional] 
**cancelledQuantity** | **String** | Quantity that was cancelled, if any. | [optional] 
**openQuantity** | **String** | Quantity that is still open, i.e., not filled or cancelled. | [optional] 
**originalQuantity** | **String** | The original quantity of the order when it was created. | [optional] 
**filledQuantity** | **String** | Quantity that has been filled so far. | [optional] 
**filledNotional** | **String** | Quote quantity that has been filled so far. | [optional] 
**lastUpdateAt** | **Date** |  | [optional] 
**openedAt** | **Date** |  | [optional] 
**inverseLeverage** | **String** |  | [optional] 
**side** | [**Side**](Side.md) |  | [optional] 
**status** | [**OrderStatus**](OrderStatus.md) |  | [optional] 
**userId** | **String** |  | [optional] 
**orderModifiers** | [**[OrderModifierKind]**](OrderModifierKind.md) |  | [optional] 
**positionId** | **String** |  | [optional] 
**orderInfo** | **String** |  | [optional] 
**goodTillDate** | **Date** |  | [optional] 
**triggerPrice** | **String** |  | [optional] 
