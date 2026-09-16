# Dora.TradingChallenge

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **String** |  | 
**name** | **String** | Trading challenge name | [optional] 
**tenantId** | **String** |  | 
**type** | [**TradingChallengeType**](TradingChallengeType.md) |  | 
**status** | [**TradingChallengeStatus**](TradingChallengeStatus.md) |  | 
**maxUsers** | **Number** |  | 
**startAt** | **Date** |  | 
**endAt** | **Date** |  | 
**initialUserBalance** | **String** |  | 
**goldPrizeQuantity** | **String** |  | 
**silverPrizeQuantity** | **String** |  | 
**bronzePrizeQuantity** | **String** |  | 
**pnlCondition** | **String** |  | 
**totalVolumeCondition** | **String** |  | 
**avgDailyVolumeCondition** | **String** |  | 
**minimumEquityPercentageCondition** | **Number** |  | 
**createdAt** | **Date** |  | 
**lastProcessedAt** | **Date** |  | [optional] 
**users** | **[String]** |  | [optional] 
**usersCount** | **Number** |  | 
**qr** | [**TradingChallengeQR**](TradingChallengeQR.md) |  | [optional] 
**worstCaseExposure** | **String** | For QR_PROMO, max_users multiplied by initial_user_balance plus max_reward_amount. | [optional] 


