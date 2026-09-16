# Dora.AffiliateReferral

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**userId** | **String** |  | 
**programId** | **String** |  | 
**referrerId** | **String** |  | 
**referrerUserId** | **String** |  | 
**signupSource** | **String** | Client-reported signup hostname. Empty means unknown. | 
**firstName** | **String** |  | 
**lastName** | **String** |  | 
**email** | **String** |  | 
**signedUpAt** | **Date** |  | 
**kycCompleted** | **Boolean** |  | 
**kycCompletedAt** | **Date** |  | 
**discordStatus** | **String** | No Discord membership integration is currently available. Unknown must not be interpreted as not joined. | 
**depositCount** | **Number** |  | 
**withdrawalCount** | **Number** |  | 
**hasTraded** | **Boolean** |  | 
**firstDepositAt** | **Date** |  | 
**lastDepositAt** | **Date** |  | 
**firstWithdrawalAt** | **Date** |  | 
**lastWithdrawalAt** | **Date** |  | 
**dailyVolumeUsd** | **String** | Sum of absolute executed FILL quantity1 on USD-quoted trades during the selected UTC day. Both buy and sell executions count, once per user-side fill. | 
**monthlyVolumeUsd** | **String** | Same executed USD quote-notional definition for the calendar month containing date. | 
**dailyRealizedPnlUsd** | **String** | Sum of realized_pnl_settlements.realized_usd created during the selected UTC day, matching the existing PnL ranking convention. Excludes unrealized PnL; this is not total account equity change. | 
**attributedAt** | **Date** | Immutable referral assignment time. Earlier activity is excluded from affiliate metrics and cash flows. | 
**monthlyRealizedPnlUsd** | **String** | Realized PnL for the UTC calendar month containing date, including only settlements at or after attributed_at. | 



## Enum: DiscordStatusEnum


* `unknown` (value: `"unknown"`)




