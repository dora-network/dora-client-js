# Dora.BulkOrderResult

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**index** | **Number** | Position of the order in the request | 
**clientOrderId** | **String** |  | [optional] 
**orderId** | **String** | Present when the order was created | [optional] 
**status** | **Number** | HTTP status the order would have received from POST /v1/orders: 201 when created | 
**error** | **String** | Present when the order was rejected | [optional] 


