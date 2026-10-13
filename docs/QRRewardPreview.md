# Dora.QRRewardPreview

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tradingChallengeId** | **String** |  | 
**state** | **String** |  | 
**currentEquity** | **String** |  | [optional] 
**promoCredit** | **String** |  | 
**eligibleProfit** | **String** |  | [optional] 
**projectedReward** | **String** |  | [optional] 
**rewardAmount** | **String** |  | [optional] 
**minRewardAmount** | **String** |  | 
**maxRewardAmount** | **String** |  | 
**rewardDeadlineAt** | **Date** |  | 
**kycCompleted** | **Boolean** |  | 
**kycUrl** | **String** |  | [optional] 
**blockers** | **[String]** |  | 



## Enum: StateEnum


* `NOT_ELIGIBLE` (value: `"NOT_ELIGIBLE"`)

* `ELIGIBLE` (value: `"ELIGIBLE"`)

* `PENDING_KYC` (value: `"PENDING_KYC"`)

* `PAID` (value: `"PAID"`)

* `LAPSED` (value: `"LAPSED"`)





## Enum: [BlockersEnum]


* `BELOW_MINIMUM_PAYOUT` (value: `"BELOW_MINIMUM_PAYOUT"`)

* `BUSTED` (value: `"BUSTED"`)

* `OTHER_CHALLENGE_FUNDED` (value: `"OTHER_CHALLENGE_FUNDED"`)

* `REWARD_DEADLINE_PASSED` (value: `"REWARD_DEADLINE_PASSED"`)

* `CHALLENGE_NOT_STARTED` (value: `"CHALLENGE_NOT_STARTED"`)

* `ALREADY_REQUESTED` (value: `"ALREADY_REQUESTED"`)

* `KYC_URL_UNAVAILABLE` (value: `"KYC_URL_UNAVAILABLE"`)




