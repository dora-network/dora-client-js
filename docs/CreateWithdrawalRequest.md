# Dora.CreateWithdrawalRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**withdrawalId** | **String** | Client-supplied idempotency key (also the on-chain correlation key). Repeating a request with the same withdrawal_id has no additional effect. | 
**toAddress** | **String** | Destination wallet address as a 0x-prefixed hex string. Must not be the zero address. | 
**quantity** | **String** | Human-decimal USDC quantity to withdraw. Must be positive and no finer than USDC&#39;s 6 on-chain decimals. | 


