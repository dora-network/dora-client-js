# Dora.RealizedPnlSettlements

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**settlements** | [**[RealizedPnlSettlement]**](RealizedPnlSettlement.md) | A list of realized PnL settlements matching the query parameters of the request | [optional] 
**userTotals** | **{String: Number}** | A map of user IDs to their total realized PnL in USD across all settlements included in the response | [optional] 
**tenantTotals** | **{String: Number}** | A map of tenant IDs to their total realized PnL in USD across all settlements included in the response | [optional] 
**userTotalsUnsettled** | **{String: Number}** | A map of user IDs to their total realized PnL in USD across unsettled settlements (where settled_at is null) included in the response | [optional] 
**tenantTotalsUnsettled** | **{String: Number}** | A map of tenant IDs to their total realized PnL in USD across unsettled settlements (where settled_at is null) included in the response | [optional] 


