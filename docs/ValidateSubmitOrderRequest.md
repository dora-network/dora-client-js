# Dora.ValidateSubmitOrderRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**quantity** | **String** |  | 
**tick** | **String** | Minimum tradable increment for the selected order book | 
**kind** | [**OrderKind**](OrderKind.md) | Must be LIMIT or MARKET | 
**side** | [**Side**](Side.md) | Must be BUY or SELL | [optional] 
**price** | **String** | If kind is LIMIT, must be &gt; 0; if MARKET it must be 0 or omitted | 
**goodTillDate** | **Date** |  | [optional] 
**inverseLeverage** | **String** |  | 
**userBalance** | **String** | User balance used to ensure they can afford the requested quantity | 
**baseAssetId** | **String** | base asset of orderbook | [optional] 
**quoteAssetId** | **String** | quote asset of orderbook | [optional] 
**clientOrderId** | **String** | An optional client-provided identifier for the order. | [optional] 
**positionAssets** | [**[PositionAsset]**](PositionAsset.md) | Full list of assets in the position with their price and collateral weight, required when inverse_leverage &lt; 1 for leverage health checks | [optional] 
**assetsConfig** | [**[AssetConfig]**](AssetConfig.md) | Configuration for the assets in the order | [optional] 
**stopLossPrice** | **String** | Stop loss price | [optional] 
**takeProfitPrice** | **String** | Take profit price | [optional] 
**restrictions** | [**TenantRestrictions**](TenantRestrictions.md) |  | [optional] 
**initialCapital** | **String** | Initial capital value in USD only used to validate sells with leverage | [optional] 


