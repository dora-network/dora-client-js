# Dora.DefaultApi

All URIs are relative to *https://staging.dora.co*

Method | HTTP request | Description
------------- | ------------- | -------------
[**approveLedgerWithdrawRequest**](DefaultApi.md#approveLedgerWithdrawRequest) | **POST** /v1/ledger/withdraw/requests/{withdrawal_id}/approve | Approve a pending withdrawal request
[**cancelAllOpenOrders**](DefaultApi.md#cancelAllOpenOrders) | **DELETE** /v1/orders | Cancel all open orders, if user passes orderbook on query param it will cancel all orders on specific orderbook, admin can cancel user&#39;s orders on specific orderbook
[**cancelLedgerWithdrawRequest**](DefaultApi.md#cancelLedgerWithdrawRequest) | **POST** /v1/ledger/withdraw/requests/{withdrawal_id}/cancel | Cancel a pending withdrawal request
[**cancelOrderById**](DefaultApi.md#cancelOrderById) | **DELETE** /v1/orders/{order_id} | Cancel an order by ID
[**checkUserEmailExists**](DefaultApi.md#checkUserEmailExists) | **GET** /v1/user/exists | Check whether a user email exists
[**claimLeverageGetAccruedInterest**](DefaultApi.md#claimLeverageGetAccruedInterest) | **POST** /v1/leverage/accrued_interest/claim | Claim current accrued leverage interest for a specific user
[**closeIsolatedPosition**](DefaultApi.md#closeIsolatedPosition) | **POST** /v1/positions/close | Close isolated positions, repaying the borrowed
[**createAPIKeyForUser**](DefaultApi.md#createAPIKeyForUser) | **POST** /v1/user/apikey | Create apikey for a user
[**createAPIKeyForUserID**](DefaultApi.md#createAPIKeyForUserID) | **POST** /v1/user/{user_id}/apikey | Create apikey for a user
[**createConditionalOrder**](DefaultApi.md#createConditionalOrder) | **POST** /v1/orders/conditional | Create a new conditional orders
[**createOrder**](DefaultApi.md#createOrder) | **POST** /v1/orders | Create a new order
[**createUser**](DefaultApi.md#createUser) | **POST** /v1/integrators/user | Create a new user
[**deleteUser**](DefaultApi.md#deleteUser) | **DELETE** /v1/user/{user_id} | Delete user by ID
[**getAPIKeysForUserID**](DefaultApi.md#getAPIKeysForUserID) | **GET** /v1/user/{user_id}/apikey | Get user&#39;s api keys: admin or integrator only
[**getAllAssetPrices**](DefaultApi.md#getAllAssetPrices) | **GET** /v1/price | Get the current price of all assets
[**getAllPositions**](DefaultApi.md#getAllPositions) | **GET** /v1/ledger/positions | Get all users&#39; positions
[**getAllWithdrawalRequests**](DefaultApi.md#getAllWithdrawalRequests) | **GET** /v1/ledger/withdraw/requests | Get all withdrawal requests
[**getAssetById**](DefaultApi.md#getAssetById) | **GET** /v1/assets/{asset_id} | Get asset by ID
[**getAssetPrice**](DefaultApi.md#getAssetPrice) | **GET** /v1/price/asset/{asset_id} | Get the current price of an asset
[**getAssetYTMById**](DefaultApi.md#getAssetYTMById) | **GET** /v1/assets/{asset_id}/ytm | Get annualized yield to maturity for a bond asset
[**getAssetsStream**](DefaultApi.md#getAssetsStream) | **GET** /v1/assets/stream | Get all inserts or updates for assets
[**getCandleData**](DefaultApi.md#getCandleData) | **GET** /v1/charts/{order_book_id}/candle | Get candlestick data for an orderbook
[**getCouponPaymentsByAssetId**](DefaultApi.md#getCouponPaymentsByAssetId) | **GET** /v1/assets/{asset_id}/coupon_payments | Get coupon payments for a bond asset
[**getL1Depth**](DefaultApi.md#getL1Depth) | **GET** /v1/orderbooks/{order_book_id}/L1 | Get the top price levels for a specific orderbook (L1 market depth)
[**getL2Depth**](DefaultApi.md#getL2Depth) | **GET** /v1/orderbooks/{order_book_id}/L2 | Get the aggregated price levels for a specific orderbook (L2 market depth)
[**getL3Depth**](DefaultApi.md#getL3Depth) | **GET** /v1/orderbooks/{order_book_id}/L3 | Get all open orders for a specific orderbook (L3 market depth)
[**getLedgerBalancesSelf**](DefaultApi.md#getLedgerBalancesSelf) | **GET** /v1/ledger/balances/self | Get your own available, locked, and borrowed assets
[**getLedgerInterestSelf**](DefaultApi.md#getLedgerInterestSelf) | **GET** /v1/ledger/interest/self | Get your own interest
[**getLedgerModule**](DefaultApi.md#getLedgerModule) | **GET** /v1/ledger/module | Get the entire module object, including unborrowed leverage assets and total leverage trackers
[**getLedgerModuleByAsset**](DefaultApi.md#getLedgerModuleByAsset) | **GET** /v1/ledger/module/{asset_id} | Get the module object for a single asset ID
[**getLedgerPositionsSelf**](DefaultApi.md#getLedgerPositionsSelf) | **GET** /v1/ledger/positions/self | Get your own positions
[**getLedgerValueSelf**](DefaultApi.md#getLedgerValueSelf) | **GET** /v1/ledger/value/self | Get your own available, locked, and borrowed USD value; and realized and unrealized PnL
[**getLedgerWithdrawRequestsBySelf**](DefaultApi.md#getLedgerWithdrawRequestsBySelf) | **GET** /v1/ledger/withdraw/requests/self | Get all pending withdrawal requests for the logged in user
[**getLedgerWithdrawRequestsByUserID**](DefaultApi.md#getLedgerWithdrawRequestsByUserID) | **GET** /v1/ledger/withdraw/requests/{user_id} | Get all pending withdrawal requests for this user
[**getOrderById**](DefaultApi.md#getOrderById) | **GET** /v1/orders/{order_id} | Get order by ID
[**getOrderbookById**](DefaultApi.md#getOrderbookById) | **GET** /v1/orderbooks/{order_book_id} | Get orderbook by ID
[**getOrderbookDepth**](DefaultApi.md#getOrderbookDepth) | **GET** /v1/orderbooks/{order_book_id}/depth | Get the aggregated price levels for a specific orderbook (L2 market depth)
[**getOrderbookOrders**](DefaultApi.md#getOrderbookOrders) | **GET** /v1/orderbooks/{order_book_id}/orders | Get all open orders for a specific orderbook (L3 market depth)
[**getOrderbookStats**](DefaultApi.md#getOrderbookStats) | **GET** /v1/orderbooks/{order_book_id}/stats | Get orderbook stats
[**getOrderbookStatsStream**](DefaultApi.md#getOrderbookStatsStream) | **GET** /v1/orderbooks/{order_book_id}/stats/stream | Orderbook stats stream
[**getOrderbookSummary**](DefaultApi.md#getOrderbookSummary) | **GET** /v1/orderbooks/{order_book_id}/summary | Get summary of an orderbook
[**getOrderbookTop**](DefaultApi.md#getOrderbookTop) | **GET** /v1/orderbooks/{order_book_id}/top | Get the top price levels for a specific orderbook (L1 market depth)
[**getPLForSelfByAccount**](DefaultApi.md#getPLForSelfByAccount) | **GET** /v1/pl/self | Get account-by-account PL breakdown for the logged in user
[**getPoolPrice**](DefaultApi.md#getPoolPrice) | **GET** /v1/price/pool/{pool_id} | Get the current price of a pool
[**getRealizedPnlSettlements**](DefaultApi.md#getRealizedPnlSettlements) | **GET** /v1/realized_pnl_settlements | Get realized P&amp;L settlements with filters
[**getTradeById**](DefaultApi.md#getTradeById) | **GET** /v1/trades/{trade_id} | Get a trade by ID
[**getTrades**](DefaultApi.md#getTrades) | **GET** /v1/trades | Get a filtered, paginated list of trades
[**getTransactionById**](DefaultApi.md#getTransactionById) | **GET** /v1/transactions/{transaction_id} | Get a transaction by ID
[**getTransactions**](DefaultApi.md#getTransactions) | **GET** /v1/transactions | Get a filtered, paginated list of transactions
[**getTransactionsSettlements**](DefaultApi.md#getTransactionsSettlements) | **GET** /v1/transactions/settlements | Get transactions settlements with filters
[**getUserById**](DefaultApi.md#getUserById) | **GET** /v1/user/{user_id} | Get user by ID (admin only)
[**getUserCouponPaymentsStream**](DefaultApi.md#getUserCouponPaymentsStream) | **GET** /v1/user/{user_id}/coupon_payments/stream | Stream user&#39;s coupon payment accruals in real time
[**getUserLedgerStream**](DefaultApi.md#getUserLedgerStream) | **GET** /v1/user/{user_id}/ledger/stream | Get a snapshot of user&#39;s ledger updates since a specific time, and opens a stream for further updates
[**getUserOrderUpdatesStream**](DefaultApi.md#getUserOrderUpdatesStream) | **GET** /v1/user/{user_id}/orders/{order_book_id}/updates/stream | Get a snapshot of user&#39;s order updates for the given order book since a specific time, and opens a stream for further updates
[**getUserOrdersUpdatesStreamAll**](DefaultApi.md#getUserOrdersUpdatesStreamAll) | **GET** /v1/user/{user_id}/orders/all/updates/stream | Get a snapshot of user&#39;s order updates across all order books since a specific time, and opens a stream for further updates
[**getUserSelf**](DefaultApi.md#getUserSelf) | **GET** /v1/user/self | Get user details for the authenticated user
[**getUserTransactionsStream**](DefaultApi.md#getUserTransactionsStream) | **GET** /v1/user/{user_id}/transactions/stream | Get a snapshot of user&#39;s executed transactions since a specific time, and opens a stream for further updates
[**getUsersAPIKeys**](DefaultApi.md#getUsersAPIKeys) | **GET** /v1/user/apikey | Get user&#39;s api keys
[**ledgerDeposit**](DefaultApi.md#ledgerDeposit) | **POST** /v1/ledger/deposit/{user_id} | Deposit assets into this user&#39;s account from the outside world
[**ledgerWithdraw**](DefaultApi.md#ledgerWithdraw) | **POST** /v1/ledger/withdraw/{user_id} | Withdraw assets from this user to the outside world
[**ledgerWithdrawRequest**](DefaultApi.md#ledgerWithdrawRequest) | **POST** /v1/ledger/withdraw/requests/{user_id} | Initiate a withdrawal request for this user to the outside world
[**ledgerWithdrawRequestSelf**](DefaultApi.md#ledgerWithdrawRequestSelf) | **POST** /v1/ledger/withdraw/requests/self | Initiate a withdrawal request for the logged in user to the outside world
[**leverageGetAccruedInterestByUser**](DefaultApi.md#leverageGetAccruedInterestByUser) | **GET** /v1/leverage/accrued_interest/self | Get current accrued leverage interest for the user
[**leverageIsolateCollateral**](DefaultApi.md#leverageIsolateCollateral) | **POST** /v1/leverage/isolate_collateral | Create an isolated position by transferring collateral to the position from the user&#39;s global collateral
[**leverageSupply**](DefaultApi.md#leverageSupply) | **POST** /v1/leverage/supply | Supply leverage for a specific asset
[**leverageUnite**](DefaultApi.md#leverageUnite) | **POST** /v1/leverage/unite | Combines all isolated positions into a single global position
[**leverageWithdraw**](DefaultApi.md#leverageWithdraw) | **POST** /v1/leverage/withdraw | Withdraw leverage for a specific asset
[**liquidityAdd**](DefaultApi.md#liquidityAdd) | **POST** /v1/liquidity/pool/{pool_id}/add | Add liquidity to a pool
[**liquiditySubtract**](DefaultApi.md#liquiditySubtract) | **POST** /v1/liquidity/pool/{pool_id}/remove | Subtract liquidity from a pool
[**listAssets**](DefaultApi.md#listAssets) | **GET** /v1/assets | List assets
[**listOrderBooks**](DefaultApi.md#listOrderBooks) | **GET** /v1/orderbooks | List order books
[**listOrders**](DefaultApi.md#listOrders) | **GET** /v1/orders | List all orders
[**listPositionAccountsSelf**](DefaultApi.md#listPositionAccountsSelf) | **GET** /v1/user/self/position_accounts | List all position accounts for the authenticated user
[**payLeverageGetAccruedInterest**](DefaultApi.md#payLeverageGetAccruedInterest) | **POST** /v1/leverage/accrued_interest/pay | Pay current accrued leverage interest for a specific user
[**rejectLedgerWithdrawRequest**](DefaultApi.md#rejectLedgerWithdrawRequest) | **POST** /v1/ledger/withdraw/requests/{withdrawal_id}/reject | Reject a pending withdrawal request
[**revokeAPIKeyForUser**](DefaultApi.md#revokeAPIKeyForUser) | **PUT** /v1/user/apikey/{key_id}/revoke | Revoke apikey for a user
[**revokeAPIKeyForUserID**](DefaultApi.md#revokeAPIKeyForUserID) | **PUT** /v1/user/{user_id}/apikey/{key_id}/revoke | Revoke apikey for a user: admin or integrator only
[**settleLeverageAccruedInterest**](DefaultApi.md#settleLeverageAccruedInterest) | **POST** /v1/leverage/accrued_interest/settle | Settle current accrued leverage interest for a specific user
[**settleRealizedPnlRecord**](DefaultApi.md#settleRealizedPnlRecord) | **PUT** /v1/realized_pnl_settlements/{settlement_id} | Mark a realized P&amp;L settlement as settled
[**settleTransactionsSettlements**](DefaultApi.md#settleTransactionsSettlements) | **PUT** /v1/transactions/settlements | Settle multiple transactions settlements in batch
[**streamAssetPrices**](DefaultApi.md#streamAssetPrices) | **GET** /v1/prices/stream | Stream real-time asset prices as map objects
[**streamCandleData**](DefaultApi.md#streamCandleData) | **GET** /v1/charts/{order_book_id}/candle/stream | Get a snapshot of candlestick data from date provided, and open a stream for real-time updates
[**streamOrderBookBalances**](DefaultApi.md#streamOrderBookBalances) | **GET** /v1/orderbooks/{order_book_id}/balances/stream | Get a snapshot of base and quote balances for an order book and open a stream for real-time updates
[**streamOrderbookOpenOrders**](DefaultApi.md#streamOrderbookOpenOrders) | **GET** /v1/orderbooks/{order_book_id}/open/stream | Get a snapshot of open orders in an order book and open a stream for real-time updates
[**streamTrades**](DefaultApi.md#streamTrades) | **GET** /v1/trades/{order_book_id}/stream | Get a snapshot of trades executed on the given order book from a specific date and open a stream for real-time updates
[**transferAvailableBalances**](DefaultApi.md#transferAvailableBalances) | **POST** /v1/positions/transfer_balances | Transfer available balance between a user&#39;s accounts (e.g. global to isolated position)
[**updateUserConfig**](DefaultApi.md#updateUserConfig) | **PUT** /v1/user/{user_id}/config | Update user configuration by ID
[**updateUserConfigSelf**](DefaultApi.md#updateUserConfigSelf) | **PUT** /v1/user/config/self | Update user configuration for the authenticated user
[**validateSubmitOrder**](DefaultApi.md#validateSubmitOrder) | **POST** /v1/orders/validate | Validate submit order request data
[**verifyUser**](DefaultApi.md#verifyUser) | **PUT** /v1/user/{user_id}/verify | Verify a user by ID



## approveLedgerWithdrawRequest

> WithdrawalInitiationResponseEnvelope approveLedgerWithdrawRequest(withdrawalId, opts)

Approve a pending withdrawal request

Approve a pending withdrawal request, allowing the transfer of assets to the outside world to proceed. Note that this does not interact with any external systems; it simply updates the status of the withdrawal request in the ledger. Actual transfer of assets must be handled separately.

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let withdrawalId = "withdrawalId_example"; // String | 
let opts = {
  'withdrawalRequestReason': new Dora.WithdrawalRequestReason() // WithdrawalRequestReason | 
};
apiInstance.approveLedgerWithdrawRequest(withdrawalId, opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **withdrawalId** | **String**|  | 
 **withdrawalRequestReason** | [**WithdrawalRequestReason**](WithdrawalRequestReason.md)|  | [optional] 

### Return type

[**WithdrawalInitiationResponseEnvelope**](WithdrawalInitiationResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## cancelAllOpenOrders

> ListOrdersResponseEnvelope cancelAllOpenOrders(opts)

Cancel all open orders, if user passes orderbook on query param it will cancel all orders on specific orderbook, admin can cancel user&#39;s orders on specific orderbook

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let opts = {
  'orderBookId': "orderBookId_example", // String | 
  'userId': "userId_example", // String | 
  'orderKind': new Dora.OrderKind() // OrderKind | 
};
apiInstance.cancelAllOpenOrders(opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | **String**|  | [optional] 
 **userId** | **String**|  | [optional] 
 **orderKind** | [**OrderKind**](.md)|  | [optional] 

### Return type

[**ListOrdersResponseEnvelope**](ListOrdersResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## cancelLedgerWithdrawRequest

> WithdrawalInitiationResponseEnvelope cancelLedgerWithdrawRequest(withdrawalId, opts)

Cancel a pending withdrawal request

Cancel a pending withdrawal request, providing an optional reason for the cancellation.

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let withdrawalId = "withdrawalId_example"; // String | 
let opts = {
  'withdrawalRequestReason': new Dora.WithdrawalRequestReason() // WithdrawalRequestReason | 
};
apiInstance.cancelLedgerWithdrawRequest(withdrawalId, opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **withdrawalId** | **String**|  | 
 **withdrawalRequestReason** | [**WithdrawalRequestReason**](WithdrawalRequestReason.md)|  | [optional] 

### Return type

[**WithdrawalInitiationResponseEnvelope**](WithdrawalInitiationResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## cancelOrderById

> CancelOrderResponseEnvelope cancelOrderById(orderId)

Cancel an order by ID

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let orderId = "orderId_example"; // String | 
apiInstance.cancelOrderById(orderId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderId** | **String**|  | 

### Return type

[**CancelOrderResponseEnvelope**](CancelOrderResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## checkUserEmailExists

> EmailExistsResponseEnvelope checkUserEmailExists(email)

Check whether a user email exists

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let email = "email_example"; // String | 
apiInstance.checkUserEmailExists(email, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email** | **String**|  | 

### Return type

[**EmailExistsResponseEnvelope**](EmailExistsResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## claimLeverageGetAccruedInterest

> ClaimLeverageAccruedInterestResponseEnvelope claimLeverageGetAccruedInterest(claimLeverageAccruedInterestRequest)

Claim current accrued leverage interest for a specific user

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let claimLeverageAccruedInterestRequest = new Dora.ClaimLeverageAccruedInterestRequest(); // ClaimLeverageAccruedInterestRequest | 
apiInstance.claimLeverageGetAccruedInterest(claimLeverageAccruedInterestRequest, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **claimLeverageAccruedInterestRequest** | [**ClaimLeverageAccruedInterestRequest**](ClaimLeverageAccruedInterestRequest.md)|  | 

### Return type

[**ClaimLeverageAccruedInterestResponseEnvelope**](ClaimLeverageAccruedInterestResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## closeIsolatedPosition

> ClosePositionResponseEnvelope closeIsolatedPosition(closePositionRequest)

Close isolated positions, repaying the borrowed

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let closePositionRequest = new Dora.ClosePositionRequest(); // ClosePositionRequest | 
apiInstance.closeIsolatedPosition(closePositionRequest, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **closePositionRequest** | [**ClosePositionRequest**](ClosePositionRequest.md)|  | 

### Return type

[**ClosePositionResponseEnvelope**](ClosePositionResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## createAPIKeyForUser

> CreateAPIKeyResponseEnvelope createAPIKeyForUser(createAPIKeyRequest)

Create apikey for a user

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let createAPIKeyRequest = new Dora.CreateAPIKeyRequest(); // CreateAPIKeyRequest | 
apiInstance.createAPIKeyForUser(createAPIKeyRequest, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createAPIKeyRequest** | [**CreateAPIKeyRequest**](CreateAPIKeyRequest.md)|  | 

### Return type

[**CreateAPIKeyResponseEnvelope**](CreateAPIKeyResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## createAPIKeyForUserID

> CreateAPIKeyResponseEnvelope createAPIKeyForUserID(userId, createAPIKeyRequest)

Create apikey for a user

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let userId = "userId_example"; // String | 
let createAPIKeyRequest = new Dora.CreateAPIKeyRequest(); // CreateAPIKeyRequest | 
apiInstance.createAPIKeyForUserID(userId, createAPIKeyRequest, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | **String**|  | 
 **createAPIKeyRequest** | [**CreateAPIKeyRequest**](CreateAPIKeyRequest.md)|  | 

### Return type

[**CreateAPIKeyResponseEnvelope**](CreateAPIKeyResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## createConditionalOrder

> CreateConditionalOrderResponseEnvelope createConditionalOrder(createConditionalOrderRequest)

Create a new conditional orders

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let createConditionalOrderRequest = new Dora.CreateConditionalOrderRequest(); // CreateConditionalOrderRequest | 
apiInstance.createConditionalOrder(createConditionalOrderRequest, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createConditionalOrderRequest** | [**CreateConditionalOrderRequest**](CreateConditionalOrderRequest.md)|  | 

### Return type

[**CreateConditionalOrderResponseEnvelope**](CreateConditionalOrderResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## createOrder

> CreateOrderResponseEnvelope createOrder(createOrderRequest)

Create a new order

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let createOrderRequest = new Dora.CreateOrderRequest(); // CreateOrderRequest | 
apiInstance.createOrder(createOrderRequest, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createOrderRequest** | [**CreateOrderRequest**](CreateOrderRequest.md)|  | 

### Return type

[**CreateOrderResponseEnvelope**](CreateOrderResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## createUser

> UserCreatedResponseEnvelope createUser(createIntegratorUserRequest)

Create a new user

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let createIntegratorUserRequest = new Dora.CreateIntegratorUserRequest(); // CreateIntegratorUserRequest | 
apiInstance.createUser(createIntegratorUserRequest, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createIntegratorUserRequest** | [**CreateIntegratorUserRequest**](CreateIntegratorUserRequest.md)|  | 

### Return type

[**UserCreatedResponseEnvelope**](UserCreatedResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteUser

> UserDeletedResponseEnvelope deleteUser(userId)

Delete user by ID

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let userId = "userId_example"; // String | 
apiInstance.deleteUser(userId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | **String**|  | 

### Return type

[**UserDeletedResponseEnvelope**](UserDeletedResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getAPIKeysForUserID

> APIKeyResponseEnvelope getAPIKeysForUserID(userId)

Get user&#39;s api keys: admin or integrator only

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let userId = "userId_example"; // String | 
apiInstance.getAPIKeysForUserID(userId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | **String**|  | 

### Return type

[**APIKeyResponseEnvelope**](APIKeyResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getAllAssetPrices

> ListAssetPriceResponseEnvelope getAllAssetPrices()

Get the current price of all assets

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
apiInstance.getAllAssetPrices((error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**ListAssetPriceResponseEnvelope**](ListAssetPriceResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getAllPositions

> AllPositionsResponseEnvelope getAllPositions()

Get all users&#39; positions

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
apiInstance.getAllPositions((error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**AllPositionsResponseEnvelope**](AllPositionsResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getAllWithdrawalRequests

> AllWithdrawalInitiationsResponseEnvelope getAllWithdrawalRequests(opts)

Get all withdrawal requests

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let opts = {
  'status': "status_example" // String | 
};
apiInstance.getAllWithdrawalRequests(opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **status** | **String**|  | [optional] 

### Return type

[**AllWithdrawalInitiationsResponseEnvelope**](AllWithdrawalInitiationsResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getAssetById

> GetAssetByIDResponseEnvelope getAssetById(assetId)

Get asset by ID

### Example

```javascript
import Dora from 'dora';

let apiInstance = new Dora.DefaultApi();
let assetId = "assetId_example"; // String | 
apiInstance.getAssetById(assetId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **assetId** | **String**|  | 

### Return type

[**GetAssetByIDResponseEnvelope**](GetAssetByIDResponseEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getAssetPrice

> AssetPriceResponseEnvelope getAssetPrice(assetId)

Get the current price of an asset

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let assetId = "assetId_example"; // String | 
apiInstance.getAssetPrice(assetId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **assetId** | **String**|  | 

### Return type

[**AssetPriceResponseEnvelope**](AssetPriceResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getAssetYTMById

> GetAssetYTMByIDResponseEnvelope getAssetYTMById(assetId)

Get annualized yield to maturity for a bond asset

### Example

```javascript
import Dora from 'dora';

let apiInstance = new Dora.DefaultApi();
let assetId = "assetId_example"; // String | 
apiInstance.getAssetYTMById(assetId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **assetId** | **String**|  | 

### Return type

[**GetAssetYTMByIDResponseEnvelope**](GetAssetYTMByIDResponseEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getAssetsStream

> [StreamAssetsEntry] getAssetsStream(opts)

Get all inserts or updates for assets

### Example

```javascript
import Dora from 'dora';

let apiInstance = new Dora.DefaultApi();
let opts = {
  'since': new Date("2013-10-20T19:20:30+01:00"), // Date | 
  'until': new Date("2013-10-20T19:20:30+01:00") // Date | 
};
apiInstance.getAssetsStream(opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **since** | **Date**|  | [optional] 
 **until** | **Date**|  | [optional] 

### Return type

[**[StreamAssetsEntry]**](StreamAssetsEntry.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getCandleData

> ListCandlesResponseEnvelope getCandleData(orderBookId, start, end, opts)

Get candlestick data for an orderbook

### Example

```javascript
import Dora from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderBookId = "orderBookId_example"; // String | 
let start = new Date("2013-10-20T19:20:30+01:00"); // Date | 
let end = new Date("2013-10-20T19:20:30+01:00"); // Date | 
let opts = {
  'resolution': new Dora.CandleResolution() // CandleResolution | 
};
apiInstance.getCandleData(orderBookId, start, end, opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | **String**|  | 
 **start** | **Date**|  | 
 **end** | **Date**|  | 
 **resolution** | [**CandleResolution**](.md)|  | [optional] 

### Return type

[**ListCandlesResponseEnvelope**](ListCandlesResponseEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getCouponPaymentsByAssetId

> ListCouponPaymentsResponseEnvelope getCouponPaymentsByAssetId(assetId)

Get coupon payments for a bond asset

### Example

```javascript
import Dora from 'dora';

let apiInstance = new Dora.DefaultApi();
let assetId = "assetId_example"; // String | 
apiInstance.getCouponPaymentsByAssetId(assetId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **assetId** | **String**|  | 

### Return type

[**ListCouponPaymentsResponseEnvelope**](ListCouponPaymentsResponseEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getL1Depth

> GetTopOfBookResponseEnvelope getL1Depth(orderBookId)

Get the top price levels for a specific orderbook (L1 market depth)

### Example

```javascript
import Dora from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderBookId = "orderBookId_example"; // String | 
apiInstance.getL1Depth(orderBookId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | **String**|  | 

### Return type

[**GetTopOfBookResponseEnvelope**](GetTopOfBookResponseEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getL2Depth

> ListOrderBookDepthResponseEnvelope getL2Depth(orderBookId)

Get the aggregated price levels for a specific orderbook (L2 market depth)

### Example

```javascript
import Dora from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderBookId = "orderBookId_example"; // String | 
apiInstance.getL2Depth(orderBookId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | **String**|  | 

### Return type

[**ListOrderBookDepthResponseEnvelope**](ListOrderBookDepthResponseEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getL3Depth

> ListOrdersResponseEnvelope getL3Depth(orderBookId)

Get all open orders for a specific orderbook (L3 market depth)

### Example

```javascript
import Dora from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderBookId = "orderBookId_example"; // String | 
apiInstance.getL3Depth(orderBookId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | **String**|  | 

### Return type

[**ListOrdersResponseEnvelope**](ListOrdersResponseEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getLedgerBalancesSelf

> UserBalanceResponseEnvelope getLedgerBalancesSelf()

Get your own available, locked, and borrowed assets

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
apiInstance.getLedgerBalancesSelf((error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**UserBalanceResponseEnvelope**](UserBalanceResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getLedgerInterestSelf

> UserInterestResponseEnvelope getLedgerInterestSelf()

Get your own interest

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
apiInstance.getLedgerInterestSelf((error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**UserInterestResponseEnvelope**](UserInterestResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getLedgerModule

> LedgerModuleResponseEnvelope getLedgerModule()

Get the entire module object, including unborrowed leverage assets and total leverage trackers

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
apiInstance.getLedgerModule((error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**LedgerModuleResponseEnvelope**](LedgerModuleResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getLedgerModuleByAsset

> LedgerModuleByAssetResponseEnvelope getLedgerModuleByAsset(assetId)

Get the module object for a single asset ID

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let assetId = "assetId_example"; // String | 
apiInstance.getLedgerModuleByAsset(assetId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **assetId** | **String**|  | 

### Return type

[**LedgerModuleByAssetResponseEnvelope**](LedgerModuleByAssetResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getLedgerPositionsSelf

> UserPositionResponseEnvelope getLedgerPositionsSelf()

Get your own positions

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
apiInstance.getLedgerPositionsSelf((error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**UserPositionResponseEnvelope**](UserPositionResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getLedgerValueSelf

> UserValueResponseEnvelope getLedgerValueSelf()

Get your own available, locked, and borrowed USD value; and realized and unrealized PnL

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
apiInstance.getLedgerValueSelf((error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**UserValueResponseEnvelope**](UserValueResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getLedgerWithdrawRequestsBySelf

> AllWithdrawalInitiationsResponseEnvelope getLedgerWithdrawRequestsBySelf(opts)

Get all pending withdrawal requests for the logged in user

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let opts = {
  'status': "status_example" // String | 
};
apiInstance.getLedgerWithdrawRequestsBySelf(opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **status** | **String**|  | [optional] 

### Return type

[**AllWithdrawalInitiationsResponseEnvelope**](AllWithdrawalInitiationsResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getLedgerWithdrawRequestsByUserID

> AllWithdrawalInitiationsResponseEnvelope getLedgerWithdrawRequestsByUserID(userId, opts)

Get all pending withdrawal requests for this user

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let userId = "userId_example"; // String | 
let opts = {
  'status': "status_example" // String | 
};
apiInstance.getLedgerWithdrawRequestsByUserID(userId, opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | **String**|  | 
 **status** | **String**|  | [optional] 

### Return type

[**AllWithdrawalInitiationsResponseEnvelope**](AllWithdrawalInitiationsResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getOrderById

> OrderResponseEnvelope getOrderById(orderId)

Get order by ID

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let orderId = "orderId_example"; // String | 
apiInstance.getOrderById(orderId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderId** | **String**|  | 

### Return type

[**OrderResponseEnvelope**](OrderResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getOrderbookById

> OrderBookResponseEnvelope getOrderbookById(orderBookId)

Get orderbook by ID

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let orderBookId = "orderBookId_example"; // String | 
apiInstance.getOrderbookById(orderBookId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | **String**|  | 

### Return type

[**OrderBookResponseEnvelope**](OrderBookResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getOrderbookDepth

> ListOrderBookDepthResponseEnvelope getOrderbookDepth(orderBookId)

Get the aggregated price levels for a specific orderbook (L2 market depth)

### Example

```javascript
import Dora from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderBookId = "orderBookId_example"; // String | 
apiInstance.getOrderbookDepth(orderBookId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | **String**|  | 

### Return type

[**ListOrderBookDepthResponseEnvelope**](ListOrderBookDepthResponseEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getOrderbookOrders

> ListOrdersResponseEnvelope getOrderbookOrders(orderBookId)

Get all open orders for a specific orderbook (L3 market depth)

### Example

```javascript
import Dora from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderBookId = "orderBookId_example"; // String | 
apiInstance.getOrderbookOrders(orderBookId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | **String**|  | 

### Return type

[**ListOrdersResponseEnvelope**](ListOrdersResponseEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getOrderbookStats

> OrderbookStatsResponseEnvelope getOrderbookStats(orderBookId)

Get orderbook stats

### Example

```javascript
import Dora from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderBookId = "orderBookId_example"; // String | 
apiInstance.getOrderbookStats(orderBookId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | **String**|  | 

### Return type

[**OrderbookStatsResponseEnvelope**](OrderbookStatsResponseEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getOrderbookStatsStream

> OrderbookStats getOrderbookStatsStream(orderBookId)

Orderbook stats stream

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let orderBookId = "orderBookId_example"; // String | 
apiInstance.getOrderbookStatsStream(orderBookId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | **String**|  | 

### Return type

[**OrderbookStats**](OrderbookStats.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getOrderbookSummary

> OrderBookSummaryResponseEnvelope getOrderbookSummary(orderBookId)

Get summary of an orderbook

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let orderBookId = "orderBookId_example"; // String | 
apiInstance.getOrderbookSummary(orderBookId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | **String**|  | 

### Return type

[**OrderBookSummaryResponseEnvelope**](OrderBookSummaryResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getOrderbookTop

> GetTopOfBookResponseEnvelope getOrderbookTop(orderBookId)

Get the top price levels for a specific orderbook (L1 market depth)

### Example

```javascript
import Dora from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderBookId = "orderBookId_example"; // String | 
apiInstance.getOrderbookTop(orderBookId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | **String**|  | 

### Return type

[**GetTopOfBookResponseEnvelope**](GetTopOfBookResponseEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getPLForSelfByAccount

> PLResponseEnvelope getPLForSelfByAccount()

Get account-by-account PL breakdown for the logged in user

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
apiInstance.getPLForSelfByAccount((error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**PLResponseEnvelope**](PLResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getPoolPrice

> PoolPriceResponseEnvelope getPoolPrice(poolId)

Get the current price of a pool

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let poolId = "poolId_example"; // String | 
apiInstance.getPoolPrice(poolId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **poolId** | **String**|  | 

### Return type

[**PoolPriceResponseEnvelope**](PoolPriceResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getRealizedPnlSettlements

> GetRealizedPnlSettlementsResponseEnvelope getRealizedPnlSettlements(opts)

Get realized P&amp;L settlements with filters

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let opts = {
  'userId': "userId_example", // String | 
  'tenantId': "tenantId_example", // String | 
  'positionId': "positionId_example", // String | 
  'createdAfter': new Date("2013-10-20T19:20:30+01:00"), // Date | 
  'settledBefore': new Date("2013-10-20T19:20:30+01:00"), // Date | 
  'isSettled': true // Boolean | 
};
apiInstance.getRealizedPnlSettlements(opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | **String**|  | [optional] 
 **tenantId** | **String**|  | [optional] 
 **positionId** | **String**|  | [optional] 
 **createdAfter** | **Date**|  | [optional] 
 **settledBefore** | **Date**|  | [optional] 
 **isSettled** | **Boolean**|  | [optional] 

### Return type

[**GetRealizedPnlSettlementsResponseEnvelope**](GetRealizedPnlSettlementsResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getTradeById

> TradeResponseEnvelope getTradeById(tradeId)

Get a trade by ID

### Example

```javascript
import Dora from 'dora';

let apiInstance = new Dora.DefaultApi();
let tradeId = "tradeId_example"; // String | 
apiInstance.getTradeById(tradeId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tradeId** | **String**|  | 

### Return type

[**TradeResponseEnvelope**](TradeResponseEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getTrades

> ListTradeResponseEnvelope getTrades(opts)

Get a filtered, paginated list of trades

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let opts = {
  'orderBookIds': ["null"], // [String] | 
  'userIds': ["null"], // [String] | 
  'start': new Date("2013-10-20T19:20:30+01:00"), // Date | 
  'end': new Date("2013-10-20T19:20:30+01:00"), // Date | 
  'page': 1, // Number | 
  'limit': 100 // Number | 
};
apiInstance.getTrades(opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookIds** | [**[String]**](String.md)|  | [optional] 
 **userIds** | [**[String]**](String.md)|  | [optional] 
 **start** | **Date**|  | [optional] 
 **end** | **Date**|  | [optional] 
 **page** | **Number**|  | [optional] [default to 1]
 **limit** | **Number**|  | [optional] [default to 100]

### Return type

[**ListTradeResponseEnvelope**](ListTradeResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getTransactionById

> TransactionResponseEnvelope getTransactionById(transactionId)

Get a transaction by ID

### Example

```javascript
import Dora from 'dora';

let apiInstance = new Dora.DefaultApi();
let transactionId = "transactionId_example"; // String | 
apiInstance.getTransactionById(transactionId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **transactionId** | **String**|  | 

### Return type

[**TransactionResponseEnvelope**](TransactionResponseEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getTransactions

> ListTransactionsResponseEnvelope getTransactions(opts)

Get a filtered, paginated list of transactions

### Example

```javascript
import Dora from 'dora';

let apiInstance = new Dora.DefaultApi();
let opts = {
  'pools': ["null"], // [String] | 
  'userIds': ["null"], // [String] | 
  'txKinds': [new Dora.TransactionKind()], // [TransactionKind] | 
  'start': new Date("2013-10-20T19:20:30+01:00"), // Date | 
  'end': new Date("2013-10-20T19:20:30+01:00"), // Date | 
  'tenantId': "tenantId_example", // String | 
  'page': 1, // Number | 
  'limit': 100 // Number | 
};
apiInstance.getTransactions(opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **pools** | [**[String]**](String.md)|  | [optional] 
 **userIds** | [**[String]**](String.md)|  | [optional] 
 **txKinds** | [**[TransactionKind]**](TransactionKind.md)|  | [optional] 
 **start** | **Date**|  | [optional] 
 **end** | **Date**|  | [optional] 
 **tenantId** | **String**|  | [optional] 
 **page** | **Number**|  | [optional] [default to 1]
 **limit** | **Number**|  | [optional] [default to 100]

### Return type

[**ListTransactionsResponseEnvelope**](ListTransactionsResponseEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getTransactionsSettlements

> TransactionsSettlementsResponseEnvelope getTransactionsSettlements(opts)

Get transactions settlements with filters

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let opts = {
  'tenantId': "tenantId_example", // String | Tenant ID to filter settlements
  'userId': "userId_example", // String | User ID to filter settlements
  'positionId': "positionId_example", // String | Position ID to filter settlements
  'txKind': "txKind_example", // String | Transaction kind to filter settlements
  'createdAfter': new Date("2013-10-20T19:20:30+01:00"), // Date | Filter settlements created after this time
  'settledBefore': new Date("2013-10-20T19:20:30+01:00"), // Date | Filter settlements settled before this time
  'isSettled': true // Boolean | Filter settlements by settlement status
};
apiInstance.getTransactionsSettlements(opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenantId** | **String**| Tenant ID to filter settlements | [optional] 
 **userId** | **String**| User ID to filter settlements | [optional] 
 **positionId** | **String**| Position ID to filter settlements | [optional] 
 **txKind** | **String**| Transaction kind to filter settlements | [optional] 
 **createdAfter** | **Date**| Filter settlements created after this time | [optional] 
 **settledBefore** | **Date**| Filter settlements settled before this time | [optional] 
 **isSettled** | **Boolean**| Filter settlements by settlement status | [optional] 

### Return type

[**TransactionsSettlementsResponseEnvelope**](TransactionsSettlementsResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getUserById

> UserEnvelope getUserById(userId)

Get user by ID (admin only)

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let userId = "userId_example"; // String | 
apiInstance.getUserById(userId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | **String**|  | 

### Return type

[**UserEnvelope**](UserEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getUserCouponPaymentsStream

> StreamUserCouponPaymentsResponse getUserCouponPaymentsStream(userId)

Stream user&#39;s coupon payment accruals in real time

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthQuery
let apiKeyAuthQuery = defaultClient.authentications['apiKeyAuthQuery'];
apiKeyAuthQuery.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthQuery.apiKeyPrefix = 'Token';

let apiInstance = new Dora.DefaultApi();
let userId = "userId_example"; // String | 
apiInstance.getUserCouponPaymentsStream(userId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | **String**|  | 

### Return type

[**StreamUserCouponPaymentsResponse**](StreamUserCouponPaymentsResponse.md)

### Authorization

[apiKeyAuthQuery](../README.md#apiKeyAuthQuery)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getUserLedgerStream

> [StreamPositionsEntry] getUserLedgerStream(userId)

Get a snapshot of user&#39;s ledger updates since a specific time, and opens a stream for further updates

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthQuery
let apiKeyAuthQuery = defaultClient.authentications['apiKeyAuthQuery'];
apiKeyAuthQuery.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthQuery.apiKeyPrefix = 'Token';

let apiInstance = new Dora.DefaultApi();
let userId = "userId_example"; // String | 
apiInstance.getUserLedgerStream(userId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | **String**|  | 

### Return type

[**[StreamPositionsEntry]**](StreamPositionsEntry.md)

### Authorization

[apiKeyAuthQuery](../README.md#apiKeyAuthQuery)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getUserOrderUpdatesStream

> [StreamOrderUpdatesEntry] getUserOrderUpdatesStream(userId, orderBookId, opts)

Get a snapshot of user&#39;s order updates for the given order book since a specific time, and opens a stream for further updates

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthQuery
let apiKeyAuthQuery = defaultClient.authentications['apiKeyAuthQuery'];
apiKeyAuthQuery.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthQuery.apiKeyPrefix = 'Token';

let apiInstance = new Dora.DefaultApi();
let userId = "userId_example"; // String | 
let orderBookId = "orderBookId_example"; // String | 
let opts = {
  'since': new Date("2013-10-20T19:20:30+01:00") // Date | 
};
apiInstance.getUserOrderUpdatesStream(userId, orderBookId, opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | **String**|  | 
 **orderBookId** | **String**|  | 
 **since** | **Date**|  | [optional] 

### Return type

[**[StreamOrderUpdatesEntry]**](StreamOrderUpdatesEntry.md)

### Authorization

[apiKeyAuthQuery](../README.md#apiKeyAuthQuery)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getUserOrdersUpdatesStreamAll

> [StreamOrderUpdatesEntry] getUserOrdersUpdatesStreamAll(userId, opts)

Get a snapshot of user&#39;s order updates across all order books since a specific time, and opens a stream for further updates

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthQuery
let apiKeyAuthQuery = defaultClient.authentications['apiKeyAuthQuery'];
apiKeyAuthQuery.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthQuery.apiKeyPrefix = 'Token';

let apiInstance = new Dora.DefaultApi();
let userId = "userId_example"; // String | 
let opts = {
  'since': new Date("2013-10-20T19:20:30+01:00") // Date | 
};
apiInstance.getUserOrdersUpdatesStreamAll(userId, opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | **String**|  | 
 **since** | **Date**|  | [optional] 

### Return type

[**[StreamOrderUpdatesEntry]**](StreamOrderUpdatesEntry.md)

### Authorization

[apiKeyAuthQuery](../README.md#apiKeyAuthQuery)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getUserSelf

> UserEnvelope getUserSelf()

Get user details for the authenticated user

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
apiInstance.getUserSelf((error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**UserEnvelope**](UserEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getUserTransactionsStream

> [StreamTransactionsEntry] getUserTransactionsStream(userId, opts)

Get a snapshot of user&#39;s executed transactions since a specific time, and opens a stream for further updates

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthQuery
let apiKeyAuthQuery = defaultClient.authentications['apiKeyAuthQuery'];
apiKeyAuthQuery.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthQuery.apiKeyPrefix = 'Token';

let apiInstance = new Dora.DefaultApi();
let userId = "userId_example"; // String | 
let opts = {
  'since': new Date("2013-10-20T19:20:30+01:00") // Date | 
};
apiInstance.getUserTransactionsStream(userId, opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | **String**|  | 
 **since** | **Date**|  | [optional] 

### Return type

[**[StreamTransactionsEntry]**](StreamTransactionsEntry.md)

### Authorization

[apiKeyAuthQuery](../README.md#apiKeyAuthQuery)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getUsersAPIKeys

> APIKeyResponseEnvelope getUsersAPIKeys()

Get user&#39;s api keys

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
apiInstance.getUsersAPIKeys((error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**APIKeyResponseEnvelope**](APIKeyResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## ledgerDeposit

> FundUserResponseEnvelope ledgerDeposit(userId, fundUserRequest)

Deposit assets into this user&#39;s account from the outside world

Deposit assets into this user&#39;s account from the outside world. Note that this does not interact with any external systems; it simply adds the amount to the user&#39;s available balance in the ledger. Actual transfer of assets must be handled separately.

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let userId = "userId_example"; // String | 
let fundUserRequest = new Dora.FundUserRequest(); // FundUserRequest | 
apiInstance.ledgerDeposit(userId, fundUserRequest, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | **String**|  | 
 **fundUserRequest** | [**FundUserRequest**](FundUserRequest.md)|  | 

### Return type

[**FundUserResponseEnvelope**](FundUserResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## ledgerWithdraw

> FundUserResponseEnvelope ledgerWithdraw(userId, defundUserRequest, opts)

Withdraw assets from this user to the outside world

Withdraw assets from this user&#39;s account to the outside world. Note that this does not interact with any external systems; it simply deducts the amount from the user&#39;s available balance in the ledger. Actual transfer of assets must be handled separately.

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let userId = "userId_example"; // String | 
let defundUserRequest = new Dora.DefundUserRequest(); // DefundUserRequest | 
let opts = {
  'status': "status_example" // String | 
};
apiInstance.ledgerWithdraw(userId, defundUserRequest, opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | **String**|  | 
 **defundUserRequest** | [**DefundUserRequest**](DefundUserRequest.md)|  | 
 **status** | **String**|  | [optional] 

### Return type

[**FundUserResponseEnvelope**](FundUserResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## ledgerWithdrawRequest

> WithdrawalInitiationResponseEnvelope ledgerWithdrawRequest(userId, defundUserRequest)

Initiate a withdrawal request for this user to the outside world

Withdraw assets from this user&#39;s account to the outside world. Note that this does not interact with any external systems; it simply deducts the amount from the user&#39;s available balance in the ledger. Actual transfer of assets must be handled separately.

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let userId = "userId_example"; // String | 
let defundUserRequest = new Dora.DefundUserRequest(); // DefundUserRequest | 
apiInstance.ledgerWithdrawRequest(userId, defundUserRequest, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | **String**|  | 
 **defundUserRequest** | [**DefundUserRequest**](DefundUserRequest.md)|  | 

### Return type

[**WithdrawalInitiationResponseEnvelope**](WithdrawalInitiationResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## ledgerWithdrawRequestSelf

> WithdrawalInitiationResponseEnvelope ledgerWithdrawRequestSelf(userId, defundUserRequest)

Initiate a withdrawal request for the logged in user to the outside world

Withdraw assets from the logged in user&#39;s account to the outside world. Note that this does not interact with any external systems; it simply deducts the amount from the user&#39;s available balance in the ledger. Actual transfer of assets must be handled separately.

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let userId = "userId_example"; // String | 
let defundUserRequest = new Dora.DefundUserRequest(); // DefundUserRequest | 
apiInstance.ledgerWithdrawRequestSelf(userId, defundUserRequest, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | **String**|  | 
 **defundUserRequest** | [**DefundUserRequest**](DefundUserRequest.md)|  | 

### Return type

[**WithdrawalInitiationResponseEnvelope**](WithdrawalInitiationResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## leverageGetAccruedInterestByUser

> CurrentLeverageAccruedInterestResponseEnvelope leverageGetAccruedInterestByUser(opts)

Get current accrued leverage interest for the user

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let opts = {
  'positionId': "positionId_example", // String | 
  'assetId': "assetId_example" // String | 
};
apiInstance.leverageGetAccruedInterestByUser(opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **positionId** | **String**|  | [optional] 
 **assetId** | **String**|  | [optional] 

### Return type

[**CurrentLeverageAccruedInterestResponseEnvelope**](CurrentLeverageAccruedInterestResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## leverageIsolateCollateral

> IsolateCollateralResponse leverageIsolateCollateral(isolateCollateralRequest)

Create an isolated position by transferring collateral to the position from the user&#39;s global collateral

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let isolateCollateralRequest = new Dora.IsolateCollateralRequest(); // IsolateCollateralRequest | 
apiInstance.leverageIsolateCollateral(isolateCollateralRequest, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **isolateCollateralRequest** | [**IsolateCollateralRequest**](IsolateCollateralRequest.md)|  | 

### Return type

[**IsolateCollateralResponse**](IsolateCollateralResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## leverageSupply

> SupplyResponseEnvelope leverageSupply(supplyRequest)

Supply leverage for a specific asset

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let supplyRequest = new Dora.SupplyRequest(); // SupplyRequest | 
apiInstance.leverageSupply(supplyRequest, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **supplyRequest** | [**SupplyRequest**](SupplyRequest.md)|  | 

### Return type

[**SupplyResponseEnvelope**](SupplyResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## leverageUnite

> UnitePositionResponseEnvelope leverageUnite(unitePositionRequest)

Combines all isolated positions into a single global position

Combines all isolated positions into a single global position

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let unitePositionRequest = new Dora.UnitePositionRequest(); // UnitePositionRequest | 
apiInstance.leverageUnite(unitePositionRequest, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **unitePositionRequest** | [**UnitePositionRequest**](UnitePositionRequest.md)|  | 

### Return type

[**UnitePositionResponseEnvelope**](UnitePositionResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## leverageWithdraw

> WithdrawResponseEnvelope leverageWithdraw(withdrawRequest)

Withdraw leverage for a specific asset

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let withdrawRequest = new Dora.WithdrawRequest(); // WithdrawRequest | 
apiInstance.leverageWithdraw(withdrawRequest, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **withdrawRequest** | [**WithdrawRequest**](WithdrawRequest.md)|  | 

### Return type

[**WithdrawResponseEnvelope**](WithdrawResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## liquidityAdd

> LiquidityResponseEnvelope liquidityAdd(poolId, liquidityRequest)

Add liquidity to a pool

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let poolId = "poolId_example"; // String | 
let liquidityRequest = new Dora.LiquidityRequest(); // LiquidityRequest | 
apiInstance.liquidityAdd(poolId, liquidityRequest, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **poolId** | **String**|  | 
 **liquidityRequest** | [**LiquidityRequest**](LiquidityRequest.md)|  | 

### Return type

[**LiquidityResponseEnvelope**](LiquidityResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## liquiditySubtract

> LiquidityResponseEnvelope liquiditySubtract(poolId, liquidityRequest)

Subtract liquidity from a pool

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let poolId = "poolId_example"; // String | 
let liquidityRequest = new Dora.LiquidityRequest(); // LiquidityRequest | 
apiInstance.liquiditySubtract(poolId, liquidityRequest, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **poolId** | **String**|  | 
 **liquidityRequest** | [**LiquidityRequest**](LiquidityRequest.md)|  | 

### Return type

[**LiquidityResponseEnvelope**](LiquidityResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## listAssets

> ResponseEnvelopeOfListAssets listAssets(opts)

List assets

### Example

```javascript
import Dora from 'dora';

let apiInstance = new Dora.DefaultApi();
let opts = {
  'createdAfter': new Date("2013-10-20T19:20:30+01:00"), // Date | 
  'createdBefore': new Date("2013-10-20T19:20:30+01:00"), // Date | 
  'assetKind': new Dora.AssetKind(), // AssetKind | Asset kind (BOND, CURRENCY, INTEREST, POOL_SHARE)
  'canAddLiquidity': true, // Boolean | 
  'canDirectBorrow': true, // Boolean | 
  'canOnboard': true, // Boolean | 
  'canTrade': true, // Boolean | 
  'canVirtualBorrow': true, // Boolean | 
  'page': 1, // Number | 
  'limit': 100 // Number | 
};
apiInstance.listAssets(opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createdAfter** | **Date**|  | [optional] 
 **createdBefore** | **Date**|  | [optional] 
 **assetKind** | [**AssetKind**](.md)| Asset kind (BOND, CURRENCY, INTEREST, POOL_SHARE) | [optional] 
 **canAddLiquidity** | **Boolean**|  | [optional] 
 **canDirectBorrow** | **Boolean**|  | [optional] 
 **canOnboard** | **Boolean**|  | [optional] 
 **canTrade** | **Boolean**|  | [optional] 
 **canVirtualBorrow** | **Boolean**|  | [optional] 
 **page** | **Number**|  | [optional] [default to 1]
 **limit** | **Number**|  | [optional] [default to 100]

### Return type

[**ResponseEnvelopeOfListAssets**](ResponseEnvelopeOfListAssets.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listOrderBooks

> ListOrderbookResponseEnvelope listOrderBooks(opts)

List order books

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let opts = {
  'status': new Dora.OrderBookStatus(), // OrderBookStatus | 
  'baseAssetId': "baseAssetId_example", // String | 
  'quoteAssetId': "quoteAssetId_example", // String | 
  'page': 1, // Number | 
  'limit': 100 // Number | 
};
apiInstance.listOrderBooks(opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **status** | [**OrderBookStatus**](.md)|  | [optional] 
 **baseAssetId** | **String**|  | [optional] 
 **quoteAssetId** | **String**|  | [optional] 
 **page** | **Number**|  | [optional] [default to 1]
 **limit** | **Number**|  | [optional] [default to 100]

### Return type

[**ListOrderbookResponseEnvelope**](ListOrderbookResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listOrders

> ListOrdersResponseEnvelope listOrders(opts)

List all orders

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let opts = {
  'orderBookId': ["null"], // [String] | 
  'kind': [new Dora.OrderKind()], // [OrderKind] | 
  'status': [new Dora.OrderStatus()], // [OrderStatus] | 
  'side': new Dora.Side(), // Side | 
  'from': new Date("2013-10-20T19:20:30+01:00"), // Date | 
  'to': new Date("2013-10-20T19:20:30+01:00"), // Date | 
  'page': 1, // Number | 
  'limit': 100 // Number | 
};
apiInstance.listOrders(opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | [**[String]**](String.md)|  | [optional] 
 **kind** | [**[OrderKind]**](OrderKind.md)|  | [optional] 
 **status** | [**[OrderStatus]**](OrderStatus.md)|  | [optional] 
 **side** | [**Side**](.md)|  | [optional] 
 **from** | **Date**|  | [optional] 
 **to** | **Date**|  | [optional] 
 **page** | **Number**|  | [optional] [default to 1]
 **limit** | **Number**|  | [optional] [default to 100]

### Return type

[**ListOrdersResponseEnvelope**](ListOrdersResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listPositionAccountsSelf

> ListPositionAccountsResponseEnvelope listPositionAccountsSelf()

List all position accounts for the authenticated user

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
apiInstance.listPositionAccountsSelf((error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**ListPositionAccountsResponseEnvelope**](ListPositionAccountsResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## payLeverageGetAccruedInterest

> PayLeverageAccruedInterestResponseEnvelope payLeverageGetAccruedInterest(payLeverageAccruedInterestRequest)

Pay current accrued leverage interest for a specific user

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let payLeverageAccruedInterestRequest = new Dora.PayLeverageAccruedInterestRequest(); // PayLeverageAccruedInterestRequest | 
apiInstance.payLeverageGetAccruedInterest(payLeverageAccruedInterestRequest, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **payLeverageAccruedInterestRequest** | [**PayLeverageAccruedInterestRequest**](PayLeverageAccruedInterestRequest.md)|  | 

### Return type

[**PayLeverageAccruedInterestResponseEnvelope**](PayLeverageAccruedInterestResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## rejectLedgerWithdrawRequest

> WithdrawalInitiationResponseEnvelope rejectLedgerWithdrawRequest(withdrawalId, withdrawalRequestReason)

Reject a pending withdrawal request

Reject a pending withdrawal request, providing a reason for the rejection. Note that this does not interact with any external systems; it simply updates the status of the withdrawal request in the ledger. Actual transfer of assets must be handled separately.

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let withdrawalId = "withdrawalId_example"; // String | 
let withdrawalRequestReason = new Dora.WithdrawalRequestReason(); // WithdrawalRequestReason | 
apiInstance.rejectLedgerWithdrawRequest(withdrawalId, withdrawalRequestReason, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **withdrawalId** | **String**|  | 
 **withdrawalRequestReason** | [**WithdrawalRequestReason**](WithdrawalRequestReason.md)|  | 

### Return type

[**WithdrawalInitiationResponseEnvelope**](WithdrawalInitiationResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## revokeAPIKeyForUser

> RevokeAPIKeyResponseEnvelope revokeAPIKeyForUser(keyId)

Revoke apikey for a user

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let keyId = "keyId_example"; // String | 
apiInstance.revokeAPIKeyForUser(keyId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **keyId** | **String**|  | 

### Return type

[**RevokeAPIKeyResponseEnvelope**](RevokeAPIKeyResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## revokeAPIKeyForUserID

> RevokeAPIKeyResponseEnvelope revokeAPIKeyForUserID(userId, keyId)

Revoke apikey for a user: admin or integrator only

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let userId = "userId_example"; // String | 
let keyId = "keyId_example"; // String | 
apiInstance.revokeAPIKeyForUserID(userId, keyId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | **String**|  | 
 **keyId** | **String**|  | 

### Return type

[**RevokeAPIKeyResponseEnvelope**](RevokeAPIKeyResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## settleLeverageAccruedInterest

> SettleLeverageAccruedInterestResponseEnvelope settleLeverageAccruedInterest(settleLeverageAccruedInterestRequest)

Settle current accrued leverage interest for a specific user

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let settleLeverageAccruedInterestRequest = new Dora.SettleLeverageAccruedInterestRequest(); // SettleLeverageAccruedInterestRequest | 
apiInstance.settleLeverageAccruedInterest(settleLeverageAccruedInterestRequest, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **settleLeverageAccruedInterestRequest** | [**SettleLeverageAccruedInterestRequest**](SettleLeverageAccruedInterestRequest.md)|  | 

### Return type

[**SettleLeverageAccruedInterestResponseEnvelope**](SettleLeverageAccruedInterestResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## settleRealizedPnlRecord

> SettleRealizedPnlRecordResponseEnvelope settleRealizedPnlRecord(settlementId)

Mark a realized P&amp;L settlement as settled

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let settlementId = "settlementId_example"; // String | 
apiInstance.settleRealizedPnlRecord(settlementId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **settlementId** | **String**|  | 

### Return type

[**SettleRealizedPnlRecordResponseEnvelope**](SettleRealizedPnlRecordResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## settleTransactionsSettlements

> TransactionsSettlementsResponse settleTransactionsSettlements(transactionsSettlementRequest)

Settle multiple transactions settlements in batch

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let transactionsSettlementRequest = new Dora.TransactionsSettlementRequest(); // TransactionsSettlementRequest | 
apiInstance.settleTransactionsSettlements(transactionsSettlementRequest, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **transactionsSettlementRequest** | [**TransactionsSettlementRequest**](TransactionsSettlementRequest.md)|  | 

### Return type

[**TransactionsSettlementsResponse**](TransactionsSettlementsResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## streamAssetPrices

> {String: AssetPrice} streamAssetPrices(opts)

Stream real-time asset prices as map objects

Opens a WebSocket stream for real-time asset price updates. First message contains all current prices, subsequent messages contain only changed prices. Data is sent as JSON objects keyed by asset ID.

### Example

```javascript
import Dora from 'dora';

let apiInstance = new Dora.DefaultApi();
let opts = {
  'since': new Date("2013-10-20T19:20:30+01:00"), // Date | 
  'assetId': "assetId_example" // String | 
};
apiInstance.streamAssetPrices(opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **since** | **Date**|  | [optional] 
 **assetId** | **String**|  | [optional] 

### Return type

[**{String: AssetPrice}**](AssetPrice.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## streamCandleData

> [StreamCandlesEntry] streamCandleData(orderBookId, opts)

Get a snapshot of candlestick data from date provided, and open a stream for real-time updates

### Example

```javascript
import Dora from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderBookId = "orderBookId_example"; // String | 
let opts = {
  'since': new Date("2013-10-20T19:20:30+01:00"), // Date | 
  'resolution': new Dora.CandleResolution() // CandleResolution | 
};
apiInstance.streamCandleData(orderBookId, opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | **String**|  | 
 **since** | **Date**|  | [optional] 
 **resolution** | [**CandleResolution**](.md)|  | [optional] 

### Return type

[**[StreamCandlesEntry]**](StreamCandlesEntry.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## streamOrderBookBalances

> [StreamOrderBookBalanceEntry] streamOrderBookBalances(orderBookId, opts)

Get a snapshot of base and quote balances for an order book and open a stream for real-time updates

### Example

```javascript
import Dora from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderBookId = "orderBookId_example"; // String | 
let opts = {
  'since': new Date("2013-10-20T19:20:30+01:00") // Date | 
};
apiInstance.streamOrderBookBalances(orderBookId, opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | **String**|  | 
 **since** | **Date**|  | [optional] 

### Return type

[**[StreamOrderBookBalanceEntry]**](StreamOrderBookBalanceEntry.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## streamOrderbookOpenOrders

> LiveOrderbook streamOrderbookOpenOrders(orderBookId, opts)

Get a snapshot of open orders in an order book and open a stream for real-time updates

### Example

```javascript
import Dora from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderBookId = "orderBookId_example"; // String | 
let opts = {
  'since': new Date("2013-10-20T19:20:30+01:00") // Date | 
};
apiInstance.streamOrderbookOpenOrders(orderBookId, opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | **String**|  | 
 **since** | **Date**|  | [optional] 

### Return type

[**LiveOrderbook**](LiveOrderbook.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## streamTrades

> [StreamTradesEntry] streamTrades(orderBookId, opts)

Get a snapshot of trades executed on the given order book from a specific date and open a stream for real-time updates

### Example

```javascript
import Dora from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderBookId = "orderBookId_example"; // String | 
let opts = {
  'since': new Date("2013-10-20T19:20:30+01:00") // Date | 
};
apiInstance.streamTrades(orderBookId, opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | **String**|  | 
 **since** | **Date**|  | [optional] 

### Return type

[**[StreamTradesEntry]**](StreamTradesEntry.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## transferAvailableBalances

> TransferBalancesResponseEnvelope transferAvailableBalances(transferBalancesRequest)

Transfer available balance between a user&#39;s accounts (e.g. global to isolated position)

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let transferBalancesRequest = new Dora.TransferBalancesRequest(); // TransferBalancesRequest | 
apiInstance.transferAvailableBalances(transferBalancesRequest, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **transferBalancesRequest** | [**TransferBalancesRequest**](TransferBalancesRequest.md)|  | 

### Return type

[**TransferBalancesResponseEnvelope**](TransferBalancesResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## updateUserConfig

> UserUpdatedResponseEnvelope updateUserConfig(userId, updateUserConfigRequest)

Update user configuration by ID

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let userId = "userId_example"; // String | 
let updateUserConfigRequest = new Dora.UpdateUserConfigRequest(); // UpdateUserConfigRequest | 
apiInstance.updateUserConfig(userId, updateUserConfigRequest, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | **String**|  | 
 **updateUserConfigRequest** | [**UpdateUserConfigRequest**](UpdateUserConfigRequest.md)|  | 

### Return type

[**UserUpdatedResponseEnvelope**](UserUpdatedResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## updateUserConfigSelf

> UserUpdatedResponseEnvelope updateUserConfigSelf(updateUserConfigRequest)

Update user configuration for the authenticated user

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let updateUserConfigRequest = new Dora.UpdateUserConfigRequest(); // UpdateUserConfigRequest | 
apiInstance.updateUserConfigSelf(updateUserConfigRequest, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **updateUserConfigRequest** | [**UpdateUserConfigRequest**](UpdateUserConfigRequest.md)|  | 

### Return type

[**UserUpdatedResponseEnvelope**](UserUpdatedResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## validateSubmitOrder

> ValidateSubmitOrderResponse validateSubmitOrder(validateSubmitOrderRequest)

Validate submit order request data

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let validateSubmitOrderRequest = new Dora.ValidateSubmitOrderRequest(); // ValidateSubmitOrderRequest | 
apiInstance.validateSubmitOrder(validateSubmitOrderRequest, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **validateSubmitOrderRequest** | [**ValidateSubmitOrderRequest**](ValidateSubmitOrderRequest.md)|  | 

### Return type

[**ValidateSubmitOrderResponse**](ValidateSubmitOrderResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## verifyUser

> UserUpdatedResponseEnvelope verifyUser(userId)

Verify a user by ID

### Example

```javascript
import Dora from 'dora';
let defaultClient = Dora.ApiClient.instance;
// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new Dora.DefaultApi();
let userId = "userId_example"; // String | 
apiInstance.verifyUser(userId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | **String**|  | 

### Return type

[**UserUpdatedResponseEnvelope**](UserUpdatedResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

