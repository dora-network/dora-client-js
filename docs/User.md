# Dora.User

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **String** |  | 
**closedAt** | **Date** |  | [optional] 
**disabledAt** | **Date** |  | [optional] 
**email** | **String** |  | 
**firstName** | **String** |  | 
**lastName** | **String** |  | 
**userName** | **String** |  | 
**countryOfDomicile** | [**CountryCode**](CountryCode.md) |  | 
**nativeAssetId** | **String** |  | 
**photoUrl** | **String** |  | [optional] 
**provider** | **String** |  | [optional] 
**providerId** | **String** |  | [optional] 
**roles** | [**[UserRole]**](UserRole.md) |  | 
**managedCompetitionIds** | **[String]** | Competition IDs this user is explicitly allowed to manage when they have COMPETITION_MANAGER role. Empty means no competition-management access. | [optional] 
**managedAffiliateProgramIds** | **[String]** | Affiliate program IDs this user is explicitly allowed to manage when they have AFFILIATE_MANAGER role. Empty means no affiliate-management access. | [optional] 
**timezone** | **String** | User&#39;s timezone, e.g., &#39;America/New_York&#39;, or an offset. | [optional] 
**timezoneOffset** | **Number** | timezone offset in seconds | [optional] 
**verifiedAt** | **Date** |  | [optional] 
**showTutorialCards** | **Boolean** |  | 
**notificationsEnabled** | **Boolean** |  | 
**tenantId** | **String** |  | 
**usedReferralCode** | **String** | Exact affiliate code this user applied at signup or later. Empty when no code has been applied; distinct from codes the user owns. | 
**allowEmailNotifications** | **Boolean** |  | 
**allowLiquidationsNotifications** | **Boolean** |  | 
**allowDepositWithdrawalNotifications** | **Boolean** |  | 
**allowOrdersNotifications** | **Boolean** |  | 
**allowCopyTrading** | **Boolean** |  | 
**kycCompletedAt** | **Date** | When the user completed KYC. Omitted/null if KYC has not been completed. Set via POST /v1/integrators/user/{user_id}/kyc. | [optional] 
**tag** | [**[UsersTag]**](UsersTag.md) | Tags assigned to the user by an admin. Set via PUT /v1/users/{user_id}/tag. | [optional] 


