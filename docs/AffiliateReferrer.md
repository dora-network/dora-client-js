# Dora.AffiliateReferrer

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **String** |  | 
**programId** | **String** |  | 
**tenantId** | **String** | Owning tenant for administration. This does not define a referral destination. | 
**userId** | **String** |  | 
**referralCode** | **String** | Current code to share; previously issued codes remain valid. Stored uppercase and unique across all programs and tenants. | 
**createdAt** | **Date** |  | 
**customizedAt** | **Date** | When the owner used their one code change; null until then. | 
**disabledAt** | **Date** | When this membership was disabled; null while enabled. | 
**disabledBy** | **String** | Actor who disabled this membership; null while enabled. | 


