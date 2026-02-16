# Dora.DefaultApi

All URIs are relative to *https://localhost:8084*

Method | HTTP request | Description
------------- | ------------- | -------------
[**cancelAllOpenOrders**](DefaultApi.md#cancelAllOpenOrders) | **DELETE** /v1/orders | Cancel all open orders, if user passes orderbook on query param it will cancel all orders on specific orderbook, admin can cancel user&#x27;s orders on specific orderbook
[**cancelOrderById**](DefaultApi.md#cancelOrderById) | **DELETE** /v1/orders/{order_id} | Cancel an order by ID
[**checkUserEmailExists**](DefaultApi.md#checkUserEmailExists) | **GET** /v1/user/exists | Check whether a user email exists
[**claimLeverageGetAccruedInterest**](DefaultApi.md#claimLeverageGetAccruedInterest) | **POST** /v1/leverage/accrued_interest/claim | Claim current accrued leverage interest for a specific user
[**closeIsolatedPosition**](DefaultApi.md#closeIsolatedPosition) | **POST** /v1/positions/close | Close isolated positions, repaying the borrowed
[**createAPIKeyForUser**](DefaultApi.md#createAPIKeyForUser) | **POST** /v1/user/apikey | Create apikey for a user
[**createAPIKeyForUserID**](DefaultApi.md#createAPIKeyForUserID) | **POST** /v1/user/{user_id}/apikey | Create apikey for a user
[**createOrder**](DefaultApi.md#createOrder) | **POST** /v1/orders | Create a new order
[**createUser**](DefaultApi.md#createUser) | **POST** /v1/integrators/user | Create a new user
[**deleteUser**](DefaultApi.md#deleteUser) | **DELETE** /v1/user/{user_id} | Delete user by ID
[**getAPIKeysForUserID**](DefaultApi.md#getAPIKeysForUserID) | **GET** /v1/user/{user_id}/apikey | Get user&#x27;s api keys: admin or integrator only
[**getAllAssetPrices**](DefaultApi.md#getAllAssetPrices) | **GET** /v1/price | Get the current price of all assets
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
[**getTradeById**](DefaultApi.md#getTradeById) | **GET** /v1/trades/{trade_id} | Get a trade by ID
[**getTrades**](DefaultApi.md#getTrades) | **GET** /v1/trades | Get a filtered, paginated list of trades
[**getTransactionById**](DefaultApi.md#getTransactionById) | **GET** /v1/transactions/{transaction_id} | Get a transaction by ID
[**getTransactions**](DefaultApi.md#getTransactions) | **GET** /v1/transactions | Get a filtered, paginated list of transactions
[**getUserById**](DefaultApi.md#getUserById) | **GET** /v1/user/{user_id} | Get user by ID (admin only)
[**getUserCouponPaymentsStream**](DefaultApi.md#getUserCouponPaymentsStream) | **GET** /v1/user/{user_id}/coupon_payments/stream | Stream user&#x27;s coupon payment accruals in real time
[**getUserLedgerStream**](DefaultApi.md#getUserLedgerStream) | **GET** /v1/user/{user_id}/ledger/stream | Get a snapshot of user&#x27;s ledger updates since a specific time, and opens a stream for further updates
[**getUserOrderUpdatesStream**](DefaultApi.md#getUserOrderUpdatesStream) | **GET** /v1/user/{user_id}/orders/{order_book_id}/updates/stream | Get a snapshot of user&#x27;s order updates for the given order book since a specific time, and opens a stream for further updates
[**getUserOrdersUpdatesStreamAll**](DefaultApi.md#getUserOrdersUpdatesStreamAll) | **GET** /v1/user/{user_id}/orders/all/updates/stream | Get a snapshot of user&#x27;s order updates across all order books since a specific time, and opens a stream for further updates
[**getUserSelf**](DefaultApi.md#getUserSelf) | **GET** /v1/user/self | Get user details for the authenticated user
[**getUserTransactionsStream**](DefaultApi.md#getUserTransactionsStream) | **GET** /v1/user/{user_id}/transactions/stream | Get a snapshot of user&#x27;s executed transactions since a specific time, and opens a stream for further updates
[**getUsersAPIKeys**](DefaultApi.md#getUsersAPIKeys) | **GET** /v1/user/apikey | Get user&#x27;s api keys
[**ledgerDeposit**](DefaultApi.md#ledgerDeposit) | **POST** /v1/ledger/deposit/{user_id} | Deposit assets into this user&#x27;s account from the outside world
[**ledgerWithdraw**](DefaultApi.md#ledgerWithdraw) | **POST** /v1/ledger/withdraw/{user_id} | Withdraw assets from this user to the outside world
[**ledgerWithdrawRequest**](DefaultApi.md#ledgerWithdrawRequest) | **POST** /v1/ledger/withdraw/requests/self | Initiate a withdrawal request for the logged in user to the outside world
[**leverageGetAccruedInterestByUser**](DefaultApi.md#leverageGetAccruedInterestByUser) | **GET** /v1/leverage/accrued_interest/self | Get current accrued leverage interest for the user
[**leverageIsolateCollateral**](DefaultApi.md#leverageIsolateCollateral) | **POST** /v1/leverage/isolate_collateral | Create an isolated position by transferring collateral to the position from the user&#x27;s global collateral
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
[**revokeAPIKeyForUser**](DefaultApi.md#revokeAPIKeyForUser) | **PUT** /v1/user/apikey/{key_id}/revoke | Revoke apikey for a user
[**revokeAPIKeyForUserID**](DefaultApi.md#revokeAPIKeyForUserID) | **PUT** /v1/user/{user_id}/apikey/{key_id}/revoke | Revoke apikey for a user: admin or integrator only
[**settleLeverageAccruedInterest**](DefaultApi.md#settleLeverageAccruedInterest) | **POST** /v1/leverage/accrued_interest/settle | Settle current accrued leverage interest for a specific user
[**streamAssetPrices**](DefaultApi.md#streamAssetPrices) | **GET** /v1/prices/stream | Stream real-time asset prices as map objects
[**streamCandleData**](DefaultApi.md#streamCandleData) | **GET** /v1/charts/{order_book_id}/candle/stream | Get a snapshot of candlestick data from date provided, and open a stream for real-time updates
[**streamOrderBookBalances**](DefaultApi.md#streamOrderBookBalances) | **GET** /v1/orderbooks/{order_book_id}/balances/stream | Get a snapshot of base and quote balances for an order book and open a stream for real-time updates
[**streamOrderbookOpenOrders**](DefaultApi.md#streamOrderbookOpenOrders) | **GET** /v1/orderbooks/{order_book_id}/open/stream | Get a snapshot of open orders in an order book and open a stream for real-time updates
[**streamTrades**](DefaultApi.md#streamTrades) | **GET** /v1/trades/{order_book_id}/stream | Get a snapshot of trades executed on the given order book from a specific date and open a stream for real-time updates
[**transferAvailableBalances**](DefaultApi.md#transferAvailableBalances) | **POST** /v1/positions/transfer_balances | Transfer available balance between a user&#x27;s accounts (e.g. global to isolated position)
[**updateUserConfig**](DefaultApi.md#updateUserConfig) | **PUT** /v1/user/{user_id}/config | Update user configuration by ID
[**updateUserConfigSelf**](DefaultApi.md#updateUserConfigSelf) | **PUT** /v1/user/config/self | Update user configuration for the authenticated user
[**validateSubmitOrder**](DefaultApi.md#validateSubmitOrder) | **POST** /v1/orders/validate | Validate submit order request data
[**verifyUser**](DefaultApi.md#verifyUser) | **PUT** /v1/user/{user_id}/verify | Verify a user by ID

<a name="cancelAllOpenOrders"></a>
# **cancelAllOpenOrders**
> ListOrdersResponse cancelAllOpenOrders(opts)

Cancel all open orders, if user passes orderbook on query param it will cancel all orders on specific orderbook, admin can cancel user&#x27;s orders on specific orderbook

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let opts = { 
  'orderBookId': null, // Object | 
  'userId': null, // Object | 
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
 **orderBookId** | [**Object**](.md)|  | [optional] 
 **userId** | [**Object**](.md)|  | [optional] 
 **orderKind** | [**OrderKind**](.md)|  | [optional] 

### Return type

[**ListOrdersResponse**](ListOrdersResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="cancelOrderById"></a>
# **cancelOrderById**
> CancelOrderResponse cancelOrderById(orderId)

Cancel an order by ID

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let orderId = null; // Object | 

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
 **orderId** | [**Object**](.md)|  | 

### Return type

[**CancelOrderResponse**](CancelOrderResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="checkUserEmailExists"></a>
# **checkUserEmailExists**
> EmailExistsResponse checkUserEmailExists(email)

Check whether a user email exists

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let email = null; // Object | 

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
 **email** | [**Object**](.md)|  | 

### Return type

[**EmailExistsResponse**](EmailExistsResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="claimLeverageGetAccruedInterest"></a>
# **claimLeverageGetAccruedInterest**
> ClaimLeverageAccruedInterestResponse claimLeverageGetAccruedInterest(body)

Claim current accrued leverage interest for a specific user

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let body = new Dora.ClaimLeverageAccruedInterestRequest(); // ClaimLeverageAccruedInterestRequest | 

apiInstance.claimLeverageGetAccruedInterest(body, (error, data, response) => {
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
 **body** | [**ClaimLeverageAccruedInterestRequest**](ClaimLeverageAccruedInterestRequest.md)|  | 

### Return type

[**ClaimLeverageAccruedInterestResponse**](ClaimLeverageAccruedInterestResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="closeIsolatedPosition"></a>
# **closeIsolatedPosition**
> ClosePositionResponse closeIsolatedPosition(body)

Close isolated positions, repaying the borrowed

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let body = new Dora.ClosePositionRequest(); // ClosePositionRequest | 

apiInstance.closeIsolatedPosition(body, (error, data, response) => {
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
 **body** | [**ClosePositionRequest**](ClosePositionRequest.md)|  | 

### Return type

[**ClosePositionResponse**](ClosePositionResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="createAPIKeyForUser"></a>
# **createAPIKeyForUser**
> CreateAPIKeyResponse createAPIKeyForUser(body)

Create apikey for a user

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let body = new Dora.CreateAPIKeyRequest(); // CreateAPIKeyRequest | 

apiInstance.createAPIKeyForUser(body, (error, data, response) => {
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
 **body** | [**CreateAPIKeyRequest**](CreateAPIKeyRequest.md)|  | 

### Return type

[**CreateAPIKeyResponse**](CreateAPIKeyResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="createAPIKeyForUserID"></a>
# **createAPIKeyForUserID**
> CreateAPIKeyResponse createAPIKeyForUserID(body, userId)

Create apikey for a user

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let body = new Dora.CreateAPIKeyRequest(); // CreateAPIKeyRequest | 
let userId = null; // Object | 

apiInstance.createAPIKeyForUserID(body, userId, (error, data, response) => {
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
 **body** | [**CreateAPIKeyRequest**](CreateAPIKeyRequest.md)|  | 
 **userId** | [**Object**](.md)|  | 

### Return type

[**CreateAPIKeyResponse**](CreateAPIKeyResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="createOrder"></a>
# **createOrder**
> CreateOrderResponse createOrder(body)

Create a new order

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let body = new Dora.CreateOrderRequest(); // CreateOrderRequest | 

apiInstance.createOrder(body, (error, data, response) => {
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
 **body** | [**CreateOrderRequest**](CreateOrderRequest.md)|  | 

### Return type

[**CreateOrderResponse**](CreateOrderResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="createUser"></a>
# **createUser**
> UserCreatedResponse createUser(body)

Create a new user

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let body = new Dora.CreateIntegratorUserRequest(); // CreateIntegratorUserRequest | 

apiInstance.createUser(body, (error, data, response) => {
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
 **body** | [**CreateIntegratorUserRequest**](CreateIntegratorUserRequest.md)|  | 

### Return type

[**UserCreatedResponse**](UserCreatedResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="deleteUser"></a>
# **deleteUser**
> UserDeletedResponse deleteUser(userId)

Delete user by ID

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let userId = null; // Object | 

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
 **userId** | [**Object**](.md)|  | 

### Return type

[**UserDeletedResponse**](UserDeletedResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getAPIKeysForUserID"></a>
# **getAPIKeysForUserID**
> GetAPIKeyResponse getAPIKeysForUserID(userId)

Get user&#x27;s api keys: admin or integrator only

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let userId = null; // Object | 

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
 **userId** | [**Object**](.md)|  | 

### Return type

[**GetAPIKeyResponse**](GetAPIKeyResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getAllAssetPrices"></a>
# **getAllAssetPrices**
> ListAssetPriceResponse getAllAssetPrices()

Get the current price of all assets

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


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

[**ListAssetPriceResponse**](ListAssetPriceResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getAssetById"></a>
# **getAssetById**
> GetAssetByIDResponse getAssetById(assetId)

Get asset by ID

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let assetId = null; // Object | 

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
 **assetId** | [**Object**](.md)|  | 

### Return type

[**GetAssetByIDResponse**](GetAssetByIDResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getAssetPrice"></a>
# **getAssetPrice**
> GetAssetPriceResponse getAssetPrice(assetId)

Get the current price of an asset

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let assetId = null; // Object | 

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
 **assetId** | [**Object**](.md)|  | 

### Return type

[**GetAssetPriceResponse**](GetAssetPriceResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getAssetYTMById"></a>
# **getAssetYTMById**
> GetAssetYTMByIDResponse getAssetYTMById(assetId)

Get annualized yield to maturity for a bond asset

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let assetId = null; // Object | 

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
 **assetId** | [**Object**](.md)|  | 

### Return type

[**GetAssetYTMByIDResponse**](GetAssetYTMByIDResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getAssetsStream"></a>
# **getAssetsStream**
> StreamAssetsResponse getAssetsStream(opts)

Get all inserts or updates for assets

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let opts = { 
  'since': null, // Object | 
  'until': null // Object | 
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
 **since** | [**Object**](.md)|  | [optional] 
 **until** | [**Object**](.md)|  | [optional] 

### Return type

[**StreamAssetsResponse**](StreamAssetsResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getCandleData"></a>
# **getCandleData**
> ListCandlesResponse getCandleData(orderBookId, opts)

Get candlestick data for an orderbook

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderBookId = null; // Object | 
let opts = { 
  'start': null, // Object | 
  'end': null, // Object | 
  'resolution': new Dora.CandleResolution() // CandleResolution | 
};
apiInstance.getCandleData(orderBookId, opts, (error, data, response) => {
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
 **orderBookId** | [**Object**](.md)|  | 
 **start** | [**Object**](.md)|  | [optional] 
 **end** | [**Object**](.md)|  | [optional] 
 **resolution** | [**CandleResolution**](.md)|  | [optional] 

### Return type

[**ListCandlesResponse**](ListCandlesResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getCouponPaymentsByAssetId"></a>
# **getCouponPaymentsByAssetId**
> ListCouponPaymentsResponse getCouponPaymentsByAssetId(assetId)

Get coupon payments for a bond asset

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let assetId = null; // Object | 

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
 **assetId** | [**Object**](.md)|  | 

### Return type

[**ListCouponPaymentsResponse**](ListCouponPaymentsResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getL1Depth"></a>
# **getL1Depth**
> GetTopOfBookResponse getL1Depth(orderBookId)

Get the top price levels for a specific orderbook (L1 market depth)

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderBookId = null; // Object | 

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
 **orderBookId** | [**Object**](.md)|  | 

### Return type

[**GetTopOfBookResponse**](GetTopOfBookResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getL2Depth"></a>
# **getL2Depth**
> ListOrderBookDepthResponse getL2Depth(orderBookId)

Get the aggregated price levels for a specific orderbook (L2 market depth)

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderBookId = null; // Object | 

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
 **orderBookId** | [**Object**](.md)|  | 

### Return type

[**ListOrderBookDepthResponse**](ListOrderBookDepthResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getL3Depth"></a>
# **getL3Depth**
> ListOrdersResponse getL3Depth(orderBookId)

Get all open orders for a specific orderbook (L3 market depth)

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderBookId = null; // Object | 

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
 **orderBookId** | [**Object**](.md)|  | 

### Return type

[**ListOrdersResponse**](ListOrdersResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getLedgerBalancesSelf"></a>
# **getLedgerBalancesSelf**
> UserBalanceResponse getLedgerBalancesSelf()

Get your own available, locked, and borrowed assets

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


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

[**UserBalanceResponse**](UserBalanceResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getLedgerInterestSelf"></a>
# **getLedgerInterestSelf**
> UserInterestResponse getLedgerInterestSelf()

Get your own interest

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


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

[**UserInterestResponse**](UserInterestResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getLedgerModule"></a>
# **getLedgerModule**
> LedgerModuleResponse getLedgerModule()

Get the entire module object, including unborrowed leverage assets and total leverage trackers

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


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

[**LedgerModuleResponse**](LedgerModuleResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getLedgerModuleByAsset"></a>
# **getLedgerModuleByAsset**
> LedgerModuleByAssetResponse getLedgerModuleByAsset(assetId)

Get the module object for a single asset ID

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let assetId = null; // Object | 

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
 **assetId** | [**Object**](.md)|  | 

### Return type

[**LedgerModuleByAssetResponse**](LedgerModuleByAssetResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getLedgerPositionsSelf"></a>
# **getLedgerPositionsSelf**
> UserPositionResponse getLedgerPositionsSelf()

Get your own positions

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


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

[**UserPositionResponse**](UserPositionResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getLedgerValueSelf"></a>
# **getLedgerValueSelf**
> UserValueResponse getLedgerValueSelf()

Get your own available, locked, and borrowed USD value; and realized and unrealized PnL

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


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

[**UserValueResponse**](UserValueResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getLedgerWithdrawRequestsBySelf"></a>
# **getLedgerWithdrawRequestsBySelf**
> AllWithdrawalInitiationsResponse getLedgerWithdrawRequestsBySelf()

Get all pending withdrawal requests for the logged in user

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
apiInstance.getLedgerWithdrawRequestsBySelf((error, data, response) => {
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

[**AllWithdrawalInitiationsResponse**](AllWithdrawalInitiationsResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderById"></a>
# **getOrderById**
> GetOrderResponse getOrderById(orderId)

Get order by ID

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let orderId = null; // Object | 

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
 **orderId** | [**Object**](.md)|  | 

### Return type

[**GetOrderResponse**](GetOrderResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderbookById"></a>
# **getOrderbookById**
> GetOrderBookResponse getOrderbookById(orderBookId)

Get orderbook by ID

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let orderBookId = null; // Object | 

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
 **orderBookId** | [**Object**](.md)|  | 

### Return type

[**GetOrderBookResponse**](GetOrderBookResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderbookDepth"></a>
# **getOrderbookDepth**
> ListOrderBookDepthResponse getOrderbookDepth(orderBookId)

Get the aggregated price levels for a specific orderbook (L2 market depth)

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderBookId = null; // Object | 

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
 **orderBookId** | [**Object**](.md)|  | 

### Return type

[**ListOrderBookDepthResponse**](ListOrderBookDepthResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderbookOrders"></a>
# **getOrderbookOrders**
> ListOrdersResponse getOrderbookOrders(orderBookId)

Get all open orders for a specific orderbook (L3 market depth)

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderBookId = null; // Object | 

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
 **orderBookId** | [**Object**](.md)|  | 

### Return type

[**ListOrdersResponse**](ListOrdersResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderbookStats"></a>
# **getOrderbookStats**
> GetOrderbookStatsResponse getOrderbookStats(orderBookId)

Get orderbook stats

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderBookId = null; // Object | 

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
 **orderBookId** | [**Object**](.md)|  | 

### Return type

[**GetOrderbookStatsResponse**](GetOrderbookStatsResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderbookStatsStream"></a>
# **getOrderbookStatsStream**
> OrderbookStats getOrderbookStatsStream(orderBookId)

Orderbook stats stream

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let orderBookId = null; // Object | 

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
 **orderBookId** | [**Object**](.md)|  | 

### Return type

[**OrderbookStats**](OrderbookStats.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderbookSummary"></a>
# **getOrderbookSummary**
> GetOrderBookSummaryResponse getOrderbookSummary(orderBookId)

Get summary of an orderbook

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let orderBookId = null; // Object | 

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
 **orderBookId** | [**Object**](.md)|  | 

### Return type

[**GetOrderBookSummaryResponse**](GetOrderBookSummaryResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderbookTop"></a>
# **getOrderbookTop**
> GetTopOfBookResponse getOrderbookTop(orderBookId)

Get the top price levels for a specific orderbook (L1 market depth)

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderBookId = null; // Object | 

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
 **orderBookId** | [**Object**](.md)|  | 

### Return type

[**GetTopOfBookResponse**](GetTopOfBookResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getPLForSelfByAccount"></a>
# **getPLForSelfByAccount**
> PLResponse getPLForSelfByAccount()

Get account-by-account PL breakdown for the logged in user

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


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

[**PLResponse**](PLResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getPoolPrice"></a>
# **getPoolPrice**
> GetPoolPriceResponse getPoolPrice(poolId)

Get the current price of a pool

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let poolId = null; // Object | 

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
 **poolId** | [**Object**](.md)|  | 

### Return type

[**GetPoolPriceResponse**](GetPoolPriceResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getTradeById"></a>
# **getTradeById**
> TradeResponse getTradeById(tradeId)

Get a trade by ID

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let tradeId = null; // Object | 

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
 **tradeId** | [**Object**](.md)|  | 

### Return type

[**TradeResponse**](TradeResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getTrades"></a>
# **getTrades**
> ListTradeResponse getTrades(opts)

Get a filtered, paginated list of trades

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let opts = { 
  'orderBookIds': null, // Object | 
  'userIds': null, // Object | 
  'start': null, // Object | 
  'end': null, // Object | 
  'page': 1, // Object | 
  'limit': 100 // Object | 
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
 **orderBookIds** | [**Object**](.md)|  | [optional] 
 **userIds** | [**Object**](.md)|  | [optional] 
 **start** | [**Object**](.md)|  | [optional] 
 **end** | [**Object**](.md)|  | [optional] 
 **page** | [**Object**](.md)|  | [optional] [default to 1]
 **limit** | [**Object**](.md)|  | [optional] [default to 100]

### Return type

[**ListTradeResponse**](ListTradeResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getTransactionById"></a>
# **getTransactionById**
> GetTransactionResponse getTransactionById(transactionId)

Get a transaction by ID

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let transactionId = null; // Object | 

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
 **transactionId** | [**Object**](.md)|  | 

### Return type

[**GetTransactionResponse**](GetTransactionResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getTransactions"></a>
# **getTransactions**
> ListTransactionsResponse getTransactions(opts)

Get a filtered, paginated list of transactions

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let opts = { 
  'pools': null, // Object | 
  'userIds': null, // Object | 
  'txKinds': null, // Object | 
  'start': null, // Object | 
  'end': null, // Object | 
  'page': 1, // Object | 
  'limit': 100 // Object | 
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
 **pools** | [**Object**](.md)|  | [optional] 
 **userIds** | [**Object**](.md)|  | [optional] 
 **txKinds** | [**Object**](.md)|  | [optional] 
 **start** | [**Object**](.md)|  | [optional] 
 **end** | [**Object**](.md)|  | [optional] 
 **page** | [**Object**](.md)|  | [optional] [default to 1]
 **limit** | [**Object**](.md)|  | [optional] [default to 100]

### Return type

[**ListTransactionsResponse**](ListTransactionsResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getUserById"></a>
# **getUserById**
> GetUserResponse getUserById(userId)

Get user by ID (admin only)

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let userId = null; // Object | 

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
 **userId** | [**Object**](.md)|  | 

### Return type

[**GetUserResponse**](GetUserResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getUserCouponPaymentsStream"></a>
# **getUserCouponPaymentsStream**
> StreamUserCouponPaymentsResponse getUserCouponPaymentsStream(userId)

Stream user&#x27;s coupon payment accruals in real time

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthQuery
let apiKeyAuthQuery = defaultClient.authentications['apiKeyAuthQuery'];
apiKeyAuthQuery.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthQuery.apiKeyPrefix = 'Token';

let apiInstance = new Dora.DefaultApi();
let userId = null; // Object | 

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
 **userId** | [**Object**](.md)|  | 

### Return type

[**StreamUserCouponPaymentsResponse**](StreamUserCouponPaymentsResponse.md)

### Authorization

[apiKeyAuthQuery](../README.md#apiKeyAuthQuery)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getUserLedgerStream"></a>
# **getUserLedgerStream**
> StreamPositionsResponse getUserLedgerStream(userId)

Get a snapshot of user&#x27;s ledger updates since a specific time, and opens a stream for further updates

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthQuery
let apiKeyAuthQuery = defaultClient.authentications['apiKeyAuthQuery'];
apiKeyAuthQuery.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthQuery.apiKeyPrefix = 'Token';

let apiInstance = new Dora.DefaultApi();
let userId = null; // Object | 

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
 **userId** | [**Object**](.md)|  | 

### Return type

[**StreamPositionsResponse**](StreamPositionsResponse.md)

### Authorization

[apiKeyAuthQuery](../README.md#apiKeyAuthQuery)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getUserOrderUpdatesStream"></a>
# **getUserOrderUpdatesStream**
> StreamOrderUpdatesResponse getUserOrderUpdatesStream(userId, orderBookId, opts)

Get a snapshot of user&#x27;s order updates for the given order book since a specific time, and opens a stream for further updates

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthQuery
let apiKeyAuthQuery = defaultClient.authentications['apiKeyAuthQuery'];
apiKeyAuthQuery.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthQuery.apiKeyPrefix = 'Token';

let apiInstance = new Dora.DefaultApi();
let userId = null; // Object | 
let orderBookId = null; // Object | 
let opts = { 
  'since': null // Object | 
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
 **userId** | [**Object**](.md)|  | 
 **orderBookId** | [**Object**](.md)|  | 
 **since** | [**Object**](.md)|  | [optional] 

### Return type

[**StreamOrderUpdatesResponse**](StreamOrderUpdatesResponse.md)

### Authorization

[apiKeyAuthQuery](../README.md#apiKeyAuthQuery)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getUserOrdersUpdatesStreamAll"></a>
# **getUserOrdersUpdatesStreamAll**
> StreamOrderUpdatesResponse getUserOrdersUpdatesStreamAll(userId, opts)

Get a snapshot of user&#x27;s order updates across all order books since a specific time, and opens a stream for further updates

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthQuery
let apiKeyAuthQuery = defaultClient.authentications['apiKeyAuthQuery'];
apiKeyAuthQuery.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthQuery.apiKeyPrefix = 'Token';

let apiInstance = new Dora.DefaultApi();
let userId = null; // Object | 
let opts = { 
  'since': null // Object | 
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
 **userId** | [**Object**](.md)|  | 
 **since** | [**Object**](.md)|  | [optional] 

### Return type

[**StreamOrderUpdatesResponse**](StreamOrderUpdatesResponse.md)

### Authorization

[apiKeyAuthQuery](../README.md#apiKeyAuthQuery)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getUserSelf"></a>
# **getUserSelf**
> GetUserResponse getUserSelf()

Get user details for the authenticated user

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


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

[**GetUserResponse**](GetUserResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getUserTransactionsStream"></a>
# **getUserTransactionsStream**
> StreamTransactionsResponse getUserTransactionsStream(userId, opts)

Get a snapshot of user&#x27;s executed transactions since a specific time, and opens a stream for further updates

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthQuery
let apiKeyAuthQuery = defaultClient.authentications['apiKeyAuthQuery'];
apiKeyAuthQuery.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthQuery.apiKeyPrefix = 'Token';

let apiInstance = new Dora.DefaultApi();
let userId = null; // Object | 
let opts = { 
  'since': null // Object | 
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
 **userId** | [**Object**](.md)|  | 
 **since** | [**Object**](.md)|  | [optional] 

### Return type

[**StreamTransactionsResponse**](StreamTransactionsResponse.md)

### Authorization

[apiKeyAuthQuery](../README.md#apiKeyAuthQuery)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getUsersAPIKeys"></a>
# **getUsersAPIKeys**
> GetAPIKeyResponse getUsersAPIKeys()

Get user&#x27;s api keys

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


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

[**GetAPIKeyResponse**](GetAPIKeyResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="ledgerDeposit"></a>
# **ledgerDeposit**
> FundUserResponse ledgerDeposit(body, userId)

Deposit assets into this user&#x27;s account from the outside world

Deposit assets into this user&#x27;s account from the outside world. Note that this does not interact with any external systems; it simply adds the amount to the user&#x27;s available balance in the ledger. Actual transfer of assets must be handled separately.

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let body = new Dora.FundUserRequest(); // FundUserRequest | 
let userId = null; // Object | 

apiInstance.ledgerDeposit(body, userId, (error, data, response) => {
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
 **body** | [**FundUserRequest**](FundUserRequest.md)|  | 
 **userId** | [**Object**](.md)|  | 

### Return type

[**FundUserResponse**](FundUserResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="ledgerWithdraw"></a>
# **ledgerWithdraw**
> FundUserResponse ledgerWithdraw(body, userId)

Withdraw assets from this user to the outside world

Withdraw assets from this user&#x27;s account to the outside world. Note that this does not interact with any external systems; it simply deducts the amount from the user&#x27;s available balance in the ledger. Actual transfer of assets must be handled separately.

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let body = new Dora.DefundUserRequest(); // DefundUserRequest | 
let userId = null; // Object | 

apiInstance.ledgerWithdraw(body, userId, (error, data, response) => {
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
 **body** | [**DefundUserRequest**](DefundUserRequest.md)|  | 
 **userId** | [**Object**](.md)|  | 

### Return type

[**FundUserResponse**](FundUserResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="ledgerWithdrawRequest"></a>
# **ledgerWithdrawRequest**
> WithdrawalInitiationResponse ledgerWithdrawRequest(body, userId)

Initiate a withdrawal request for the logged in user to the outside world

Withdraw assets from the logged in user&#x27;s account to the outside world. Note that this does not interact with any external systems; it simply deducts the amount from the user&#x27;s available balance in the ledger. Actual transfer of assets must be handled separately.

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let body = new Dora.DefundUserRequest(); // DefundUserRequest | 
let userId = null; // Object | 

apiInstance.ledgerWithdrawRequest(body, userId, (error, data, response) => {
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
 **body** | [**DefundUserRequest**](DefundUserRequest.md)|  | 
 **userId** | [**Object**](.md)|  | 

### Return type

[**WithdrawalInitiationResponse**](WithdrawalInitiationResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageGetAccruedInterestByUser"></a>
# **leverageGetAccruedInterestByUser**
> CurrentLeverageAccruedInterestResponse leverageGetAccruedInterestByUser(opts)

Get current accrued leverage interest for the user

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let opts = { 
  'positionId': null, // Object | 
  'assetId': null // Object | 
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
 **positionId** | [**Object**](.md)|  | [optional] 
 **assetId** | [**Object**](.md)|  | [optional] 

### Return type

[**CurrentLeverageAccruedInterestResponse**](CurrentLeverageAccruedInterestResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="leverageIsolateCollateral"></a>
# **leverageIsolateCollateral**
> IsolateCollateralResponse leverageIsolateCollateral(body)

Create an isolated position by transferring collateral to the position from the user&#x27;s global collateral

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let body = new Dora.IsolateCollateralRequest(); // IsolateCollateralRequest | 

apiInstance.leverageIsolateCollateral(body, (error, data, response) => {
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
 **body** | [**IsolateCollateralRequest**](IsolateCollateralRequest.md)|  | 

### Return type

[**IsolateCollateralResponse**](IsolateCollateralResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageSupply"></a>
# **leverageSupply**
> SupplyResponse leverageSupply(body)

Supply leverage for a specific asset

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let body = new Dora.SupplyRequest(); // SupplyRequest | 

apiInstance.leverageSupply(body, (error, data, response) => {
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
 **body** | [**SupplyRequest**](SupplyRequest.md)|  | 

### Return type

[**SupplyResponse**](SupplyResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageUnite"></a>
# **leverageUnite**
> UnitePositionResponse leverageUnite(body)

Combines all isolated positions into a single global position

Combines all isolated positions into a single global position

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let body = new Dora.UnitePositionRequest(); // UnitePositionRequest | 

apiInstance.leverageUnite(body, (error, data, response) => {
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
 **body** | [**UnitePositionRequest**](UnitePositionRequest.md)|  | 

### Return type

[**UnitePositionResponse**](UnitePositionResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageWithdraw"></a>
# **leverageWithdraw**
> WithdrawResponse leverageWithdraw(body)

Withdraw leverage for a specific asset

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let body = new Dora.WithdrawRequest(); // WithdrawRequest | 

apiInstance.leverageWithdraw(body, (error, data, response) => {
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
 **body** | [**WithdrawRequest**](WithdrawRequest.md)|  | 

### Return type

[**WithdrawResponse**](WithdrawResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="liquidityAdd"></a>
# **liquidityAdd**
> LiquidityResponse liquidityAdd(body, poolId)

Add liquidity to a pool

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let body = new Dora.LiquidityRequest(); // LiquidityRequest | 
let poolId = null; // Object | 

apiInstance.liquidityAdd(body, poolId, (error, data, response) => {
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
 **body** | [**LiquidityRequest**](LiquidityRequest.md)|  | 
 **poolId** | [**Object**](.md)|  | 

### Return type

[**LiquidityResponse**](LiquidityResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="liquiditySubtract"></a>
# **liquiditySubtract**
> LiquidityResponse liquiditySubtract(body, poolId)

Subtract liquidity from a pool

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let body = new Dora.LiquidityRequest(); // LiquidityRequest | 
let poolId = null; // Object | 

apiInstance.liquiditySubtract(body, poolId, (error, data, response) => {
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
 **body** | [**LiquidityRequest**](LiquidityRequest.md)|  | 
 **poolId** | [**Object**](.md)|  | 

### Return type

[**LiquidityResponse**](LiquidityResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="listAssets"></a>
# **listAssets**
> ListAssetsResponse listAssets(opts)

List assets

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let opts = { 
  'createdAfter': null, // Object | 
  'createdBefore': null, // Object | 
  'assetKind': new Dora.AssetKind(), // AssetKind | Asset kind (BOND, CURRENCY, INTEREST, POOL_SHARE)
  'canAddLiquidity': null, // Object | 
  'canDirectBorrow': null, // Object | 
  'canOnboard': null, // Object | 
  'canTrade': null, // Object | 
  'canVirtualBorrow': null, // Object | 
  'page': 1, // Object | 
  'limit': 100 // Object | 
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
 **createdAfter** | [**Object**](.md)|  | [optional] 
 **createdBefore** | [**Object**](.md)|  | [optional] 
 **assetKind** | [**AssetKind**](.md)| Asset kind (BOND, CURRENCY, INTEREST, POOL_SHARE) | [optional] 
 **canAddLiquidity** | [**Object**](.md)|  | [optional] 
 **canDirectBorrow** | [**Object**](.md)|  | [optional] 
 **canOnboard** | [**Object**](.md)|  | [optional] 
 **canTrade** | [**Object**](.md)|  | [optional] 
 **canVirtualBorrow** | [**Object**](.md)|  | [optional] 
 **page** | [**Object**](.md)|  | [optional] [default to 1]
 **limit** | [**Object**](.md)|  | [optional] [default to 100]

### Return type

[**ListAssetsResponse**](ListAssetsResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="listOrderBooks"></a>
# **listOrderBooks**
> ListOrderBooksResponse listOrderBooks(opts)

List order books

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let opts = { 
  'status': new Dora.OrderBookStatus(), // OrderBookStatus | 
  'baseAssetId': null, // Object | 
  'quoteAssetId': null, // Object | 
  'page': 1, // Object | 
  'limit': 100 // Object | 
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
 **baseAssetId** | [**Object**](.md)|  | [optional] 
 **quoteAssetId** | [**Object**](.md)|  | [optional] 
 **page** | [**Object**](.md)|  | [optional] [default to 1]
 **limit** | [**Object**](.md)|  | [optional] [default to 100]

### Return type

[**ListOrderBooksResponse**](ListOrderBooksResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="listOrders"></a>
# **listOrders**
> ListOrdersResponse listOrders(opts)

List all orders

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let opts = { 
  'orderBookId': null, // Object | 
  'kind': null, // Object | 
  'status': null, // Object | 
  'side': new Dora.Side(), // Side | 
  'from': null, // Object | 
  'to': null, // Object | 
  'page': 1, // Object | 
  'limit': 100 // Object | 
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
 **orderBookId** | [**Object**](.md)|  | [optional] 
 **kind** | [**Object**](.md)|  | [optional] 
 **status** | [**Object**](.md)|  | [optional] 
 **side** | [**Side**](.md)|  | [optional] 
 **from** | [**Object**](.md)|  | [optional] 
 **to** | [**Object**](.md)|  | [optional] 
 **page** | [**Object**](.md)|  | [optional] [default to 1]
 **limit** | [**Object**](.md)|  | [optional] [default to 100]

### Return type

[**ListOrdersResponse**](ListOrdersResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="listPositionAccountsSelf"></a>
# **listPositionAccountsSelf**
> ListPositionAccountsResponse listPositionAccountsSelf()

List all position accounts for the authenticated user

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


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

[**ListPositionAccountsResponse**](ListPositionAccountsResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="payLeverageGetAccruedInterest"></a>
# **payLeverageGetAccruedInterest**
> PayLeverageAccruedInterestResponse payLeverageGetAccruedInterest(body)

Pay current accrued leverage interest for a specific user

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let body = new Dora.PayLeverageAccruedInterestRequest(); // PayLeverageAccruedInterestRequest | 

apiInstance.payLeverageGetAccruedInterest(body, (error, data, response) => {
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
 **body** | [**PayLeverageAccruedInterestRequest**](PayLeverageAccruedInterestRequest.md)|  | 

### Return type

[**PayLeverageAccruedInterestResponse**](PayLeverageAccruedInterestResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="revokeAPIKeyForUser"></a>
# **revokeAPIKeyForUser**
> RevokeAPIKeyResponse revokeAPIKeyForUser(keyId)

Revoke apikey for a user

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let keyId = null; // Object | 

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
 **keyId** | [**Object**](.md)|  | 

### Return type

[**RevokeAPIKeyResponse**](RevokeAPIKeyResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="revokeAPIKeyForUserID"></a>
# **revokeAPIKeyForUserID**
> RevokeAPIKeyResponse revokeAPIKeyForUserID(userId, keyId)

Revoke apikey for a user: admin or integrator only

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let userId = null; // Object | 
let keyId = null; // Object | 

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
 **userId** | [**Object**](.md)|  | 
 **keyId** | [**Object**](.md)|  | 

### Return type

[**RevokeAPIKeyResponse**](RevokeAPIKeyResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="settleLeverageAccruedInterest"></a>
# **settleLeverageAccruedInterest**
> SettleLeverageAccruedInterestResponse settleLeverageAccruedInterest(body)

Settle current accrued leverage interest for a specific user

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let body = new Dora.SettleLeverageAccruedInterestRequest(); // SettleLeverageAccruedInterestRequest | 

apiInstance.settleLeverageAccruedInterest(body, (error, data, response) => {
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
 **body** | [**SettleLeverageAccruedInterestRequest**](SettleLeverageAccruedInterestRequest.md)|  | 

### Return type

[**SettleLeverageAccruedInterestResponse**](SettleLeverageAccruedInterestResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="streamAssetPrices"></a>
# **streamAssetPrices**
> StreamAssetPricesResponse streamAssetPrices(opts)

Stream real-time asset prices as map objects

Opens a WebSocket stream for real-time asset price updates. First message contains all current prices, subsequent messages contain only changed prices. Data is sent as JSON objects keyed by asset ID.

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let opts = { 
  'since': null, // Object | 
  'assetId': null // Object | 
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
 **since** | [**Object**](.md)|  | [optional] 
 **assetId** | [**Object**](.md)|  | [optional] 

### Return type

[**StreamAssetPricesResponse**](StreamAssetPricesResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="streamCandleData"></a>
# **streamCandleData**
> StreamCandlesResponse streamCandleData(orderBookId, opts)

Get a snapshot of candlestick data from date provided, and open a stream for real-time updates

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderBookId = null; // Object | 
let opts = { 
  'since': null, // Object | 
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
 **orderBookId** | [**Object**](.md)|  | 
 **since** | [**Object**](.md)|  | [optional] 
 **resolution** | [**CandleResolution**](.md)|  | [optional] 

### Return type

[**StreamCandlesResponse**](StreamCandlesResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="streamOrderBookBalances"></a>
# **streamOrderBookBalances**
> StreamOrderBookBalancesResponse streamOrderBookBalances(orderBookId, opts)

Get a snapshot of base and quote balances for an order book and open a stream for real-time updates

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderBookId = null; // Object | 
let opts = { 
  'since': null // Object | 
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
 **orderBookId** | [**Object**](.md)|  | 
 **since** | [**Object**](.md)|  | [optional] 

### Return type

[**StreamOrderBookBalancesResponse**](StreamOrderBookBalancesResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="streamOrderbookOpenOrders"></a>
# **streamOrderbookOpenOrders**
> LiveOrderbook streamOrderbookOpenOrders(orderBookId, opts)

Get a snapshot of open orders in an order book and open a stream for real-time updates

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderBookId = null; // Object | 
let opts = { 
  'since': null // Object | 
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
 **orderBookId** | [**Object**](.md)|  | 
 **since** | [**Object**](.md)|  | [optional] 

### Return type

[**LiveOrderbook**](LiveOrderbook.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="streamTrades"></a>
# **streamTrades**
> StreamTradesResponse streamTrades(orderBookId, opts)

Get a snapshot of trades executed on the given order book from a specific date and open a stream for real-time updates

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderBookId = null; // Object | 
let opts = { 
  'since': null // Object | 
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
 **orderBookId** | [**Object**](.md)|  | 
 **since** | [**Object**](.md)|  | [optional] 

### Return type

[**StreamTradesResponse**](StreamTradesResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="transferAvailableBalances"></a>
# **transferAvailableBalances**
> TransferBalancesResponse transferAvailableBalances(body)

Transfer available balance between a user&#x27;s accounts (e.g. global to isolated position)

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let body = new Dora.TransferBalancesRequest(); // TransferBalancesRequest | 

apiInstance.transferAvailableBalances(body, (error, data, response) => {
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
 **body** | [**TransferBalancesRequest**](TransferBalancesRequest.md)|  | 

### Return type

[**TransferBalancesResponse**](TransferBalancesResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="updateUserConfig"></a>
# **updateUserConfig**
> UserUpdatedResponse updateUserConfig(body, userId)

Update user configuration by ID

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let body = new Dora.UpdateUserConfigRequest(); // UpdateUserConfigRequest | 
let userId = null; // Object | 

apiInstance.updateUserConfig(body, userId, (error, data, response) => {
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
 **body** | [**UpdateUserConfigRequest**](UpdateUserConfigRequest.md)|  | 
 **userId** | [**Object**](.md)|  | 

### Return type

[**UserUpdatedResponse**](UserUpdatedResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="updateUserConfigSelf"></a>
# **updateUserConfigSelf**
> UserUpdatedResponse updateUserConfigSelf(body)

Update user configuration for the authenticated user

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let body = new Dora.UpdateUserConfigRequest(); // UpdateUserConfigRequest | 

apiInstance.updateUserConfigSelf(body, (error, data, response) => {
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
 **body** | [**UpdateUserConfigRequest**](UpdateUserConfigRequest.md)|  | 

### Return type

[**UserUpdatedResponse**](UserUpdatedResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="validateSubmitOrder"></a>
# **validateSubmitOrder**
> ValidateSubmitOrderResponse validateSubmitOrder(body)

Validate submit order request data

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let body = new Dora.ValidateSubmitOrderRequest(); // ValidateSubmitOrderRequest | 

apiInstance.validateSubmitOrder(body, (error, data, response) => {
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
 **body** | [**ValidateSubmitOrderRequest**](ValidateSubmitOrderRequest.md)|  | 

### Return type

[**ValidateSubmitOrderResponse**](ValidateSubmitOrderResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="verifyUser"></a>
# **verifyUser**
> UserUpdatedResponse verifyUser(userId)

Verify a user by ID

### Example
```javascript
import {Dora} from 'dora';
let defaultClient = Dora.ApiClient.instance;

// Configure API key authorization: apiKeyAuthHeader
let apiKeyAuthHeader = defaultClient.authentications['apiKeyAuthHeader'];
apiKeyAuthHeader.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.apiKeyPrefix = 'Token';


let apiInstance = new Dora.DefaultApi();
let userId = null; // Object | 

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
 **userId** | [**Object**](.md)|  | 

### Return type

[**UserUpdatedResponse**](UserUpdatedResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

