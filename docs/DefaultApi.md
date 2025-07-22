# Dora.DefaultApi

All URIs are relative to *https://localhost:8084*

Method | HTTP request | Description
------------- | ------------- | -------------
[**cancelAllOpenOrders**](DefaultApi.md#cancelAllOpenOrders) | **DELETE** /v1/orders | Cancel all open orders
[**cancelOrderById**](DefaultApi.md#cancelOrderById) | **DELETE** /v1/orders/{order_id} | Cancel an order by ID
[**createOrder**](DefaultApi.md#createOrder) | **POST** /v1/orders | Create a new order
[**deleteUser**](DefaultApi.md#deleteUser) | **DELETE** /v1/user/{user_id} | Delete user by ID
[**getAllAssetPrices**](DefaultApi.md#getAllAssetPrices) | **GET** /v1/price | Get the current price of all assets
[**getAssetById**](DefaultApi.md#getAssetById) | **GET** /v1/assets/{id} | Get asset by ID
[**getAssetPrice**](DefaultApi.md#getAssetPrice) | **GET** /v1/price/asset/{asset_id} | Get the current price of an asset
[**getCandleData**](DefaultApi.md#getCandleData) | **GET** /v1/charts/candle/{orderbook} | Get candlestick data for an orderbook
[**getCouponsByAssetId**](DefaultApi.md#getCouponsByAssetId) | **GET** /v1/assets/{id}/coupons | Get coupons for a bond asset
[**getL1Depth**](DefaultApi.md#getL1Depth) | **GET** /v1/orderbooks/{orderbook_id}/L1 | Get the top price levels for a specific orderbook (L1 market depth)
[**getL2Depth**](DefaultApi.md#getL2Depth) | **GET** /v1/orderbooks/{orderbook_id}/L2 | Get the aggregated price levels for a specific orderbook (L2 market depth)
[**getL3Depth**](DefaultApi.md#getL3Depth) | **GET** /v1/orderbooks/{orderbook_id}/L3 | Get all open orders for a specific orderbook (L3 market depth)
[**getLedgerBalancesSelf**](DefaultApi.md#getLedgerBalancesSelf) | **GET** /v1/ledger/balances/self | Get your own available, locked, and borrowed assets
[**getLedgerInterestSelf**](DefaultApi.md#getLedgerInterestSelf) | **GET** /v1/ledger/interest/self | Get your own interest
[**getLedgerModule**](DefaultApi.md#getLedgerModule) | **GET** /v1/ledger/module | Get the entire module object, including unborrowed leverage assets and total leverage trackers
[**getLedgerModuleByAsset**](DefaultApi.md#getLedgerModuleByAsset) | **GET** /v1/ledger/module/{asset_id} | Get the module object for a single asset ID
[**getLedgerPositionsSelf**](DefaultApi.md#getLedgerPositionsSelf) | **GET** /v1/ledger/positions/self | Get your own positions
[**getLedgerValueSelf**](DefaultApi.md#getLedgerValueSelf) | **GET** /v1/ledger/value/self | Get your own available, locked, and borrowed USD value; and realized and unrealized PnL
[**getOrderById**](DefaultApi.md#getOrderById) | **GET** /v1/orders/{order_id} | Get order by ID
[**getOrderbookBBO**](DefaultApi.md#getOrderbookBBO) | **GET** /v1/orderbooks/{orderbook_id}/bbo | Get the top price levels for a specific orderbook (L1 market depth)
[**getOrderbookById**](DefaultApi.md#getOrderbookById) | **GET** /v1/orderbooks/{orderbook_id} | Get orderbook by ID
[**getOrderbookDepth**](DefaultApi.md#getOrderbookDepth) | **GET** /v1/orderbooks/{orderbook_id}/depth | Get the aggregated price levels for a specific orderbook (L2 market depth)
[**getOrderbookOrders**](DefaultApi.md#getOrderbookOrders) | **GET** /v1/orderbooks/{orderbook_id}/orders | Get all open orders for a specific orderbook (L3 market depth)
[**getOrderbookSummary**](DefaultApi.md#getOrderbookSummary) | **GET** /v1/orderbooks/{orderbook_id}/summary | Get summary of an orderbook
[**getOrderbookTop**](DefaultApi.md#getOrderbookTop) | **GET** /v1/orderbooks/{orderbook_id}/top | Get the top price levels for a specific orderbook (L1 market depth)
[**getPoolPrice**](DefaultApi.md#getPoolPrice) | **GET** /v1/price/pool/{pool_id} | Get the current price of a pool
[**getTradeById**](DefaultApi.md#getTradeById) | **GET** /v1/trade/{trade_id} | Get a trade by ID
[**getTrades**](DefaultApi.md#getTrades) | **GET** /v1/trade | Get a filtered, paginated list of trades
[**getTransactionById**](DefaultApi.md#getTransactionById) | **GET** /v1/transactions/{id} | Get a transaction by ID
[**getTransactions**](DefaultApi.md#getTransactions) | **GET** /v1/transactions | Get a filtered, paginated list of transactions
[**getUserById**](DefaultApi.md#getUserById) | **GET** /v1/user/{user_id} | Get user by ID
[**getUserLedgerStream**](DefaultApi.md#getUserLedgerStream) | **GET** /v1/user/{user_id}/ledger/stream | Get a snapshot of user&#x27;s ledger updates since a specific time, and opens a stream for further updates
[**getUserOrdersStream**](DefaultApi.md#getUserOrdersStream) | **GET** /v1/user/{user_id}/orders/{orderbook_id}/stream | Get a snapshot of user&#x27;s order updates for the given order book since a specific time, and opens a stream for further updates
[**getUserOrdersStreamAll**](DefaultApi.md#getUserOrdersStreamAll) | **GET** /v1/user/{user_id}/orders/all/stream | Get a snapshot of user&#x27;s order updates since a specific time, and opens a stream for further updates
[**getUserSelf**](DefaultApi.md#getUserSelf) | **GET** /v1/user/self | Get user details for the authenticated user
[**getUserTransactionsStream**](DefaultApi.md#getUserTransactionsStream) | **GET** /v1/user/{user_id}/transactions/stream | Get a snapshot of user&#x27;s executed transactions since a specific time, and opens a stream for further updates
[**ledgerDeposit**](DefaultApi.md#ledgerDeposit) | **POST** /v1/ledger/deposit | Deposit assets into your account from the outside world
[**ledgerWithdraw**](DefaultApi.md#ledgerWithdraw) | **POST** /v1/ledger/withdraw | Withdraw assets from your account to the outside world
[**leverageBorrow**](DefaultApi.md#leverageBorrow) | **POST** /v1/leverage/borrow | Directly borrow assets
[**leverageCollateralize**](DefaultApi.md#leverageCollateralize) | **POST** /v1/leverage/collateralize | Move supplied and available to supplied_collateral and collateral, for a specified position
[**leverageDeCollateralize**](DefaultApi.md#leverageDeCollateralize) | **POST** /v1/leverage/de-collateralize | Move collateral and supplied_collateral to available and supplied, for a specified position.
[**leverageIsolateCollateral**](DefaultApi.md#leverageIsolateCollateral) | **POST** /v1/leverage/isolate_collateral | Create an isolated position by transferring collateral to the position from the user&#x27;s global collateral
[**leverageIsolatePosition**](DefaultApi.md#leverageIsolatePosition) | **POST** /v1/leverage/isolate_position | Create an isolated position using all collateral, supplied_collateral, and borrows from the user&#x27;s global position
[**leverageRepay**](DefaultApi.md#leverageRepay) | **POST** /v1/leverage/repay | Repay borrowed assets
[**leverageSupply**](DefaultApi.md#leverageSupply) | **POST** /v1/leverage/supply | Supply leverage for a specific asset
[**leverageUnite**](DefaultApi.md#leverageUnite) | **POST** /v1/leverage/unite | Combines all isolated positions into a single global position
[**leverageWithdraw**](DefaultApi.md#leverageWithdraw) | **POST** /v1/leverage/withdraw | Withdraw leverage for a specific asset
[**liquidityAdd**](DefaultApi.md#liquidityAdd) | **POST** /v1/liquidity/pool/{pool_id}/add | Add liquidity to a pool
[**liquiditySubtract**](DefaultApi.md#liquiditySubtract) | **POST** /v1/liquidity/pool/{pool_id}/subtract | Subtract liquidity from a pool
[**listAssets**](DefaultApi.md#listAssets) | **GET** /v1/assets | List assets
[**listOrderBooks**](DefaultApi.md#listOrderBooks) | **GET** /v1/orderbooks | List order books
[**listOrders**](DefaultApi.md#listOrders) | **GET** /v1/orders | List all orders
[**streamAssetPrices**](DefaultApi.md#streamAssetPrices) | **GET** /v1/price/stream | Get a snapshot of asset prices from a specific date and open a stream for real-time updates
[**streamCandleData**](DefaultApi.md#streamCandleData) | **GET** /v1/charts/candle/stream/{orderbook} | Get a snapshot of candlestick data from date provided, and open a stream for real-time updates
[**streamOrderBookBalances**](DefaultApi.md#streamOrderBookBalances) | **GET** /v1/orderbooks/{orderbook_id}/stream/balances | Get a snapshot of base and quote balances for an order book and open a stream for real-time updates
[**streamOrderbookOpenOrders**](DefaultApi.md#streamOrderbookOpenOrders) | **GET** /v1/orderbooks/{orderbook_id}/stream/open | Get a snapshot of open orders in an order book and open a stream for real-time updates
[**streamTrades**](DefaultApi.md#streamTrades) | **GET** /v1/trade/{orderbook_id}/stream | Get a snapshot of trades from a specific date and open a stream for real-time updates
[**updateUserConfig**](DefaultApi.md#updateUserConfig) | **PUT** /v1/user/{user_id}/config | Update user configuration by ID
[**updateUserConfigSelf**](DefaultApi.md#updateUserConfigSelf) | **PUT** /v1/user/config/self | Update user configuration for the authenticated user
[**verifyUser**](DefaultApi.md#verifyUser) | **PUT** /v1/user/{user_id}/verify | Verify a user by ID

<a name="cancelAllOpenOrders"></a>
# **cancelAllOpenOrders**
> InlineResponse20015 cancelAllOpenOrders()

Cancel all open orders

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
apiInstance.cancelAllOpenOrders((error, data, response) => {
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

[**InlineResponse20015**](InlineResponse20015.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="cancelOrderById"></a>
# **cancelOrderById**
> InlineResponse204 cancelOrderById(orderId)

Cancel an order by ID

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderId = "38400000-8cf0-11bd-b23e-10b96e4ef00d"; // String | 

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
 **orderId** | [**String**](.md)|  | 

### Return type

[**InlineResponse204**](InlineResponse204.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="createOrder"></a>
# **createOrder**
> OrderId createOrder(body)

Create a new order

### Example
```javascript
import {Dora} from 'dora';

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

[**OrderId**](OrderId.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="deleteUser"></a>
# **deleteUser**
> InlineResponse2004 deleteUser(userId)

Delete user by ID

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let userId = "38400000-8cf0-11bd-b23e-10b96e4ef00d"; // String | 

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
 **userId** | [**String**](.md)|  | 

### Return type

[**InlineResponse2004**](InlineResponse2004.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getAllAssetPrices"></a>
# **getAllAssetPrices**
> InlineResponse20028 getAllAssetPrices()

Get the current price of all assets

### Example
```javascript
import {Dora} from 'dora';

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

[**InlineResponse20028**](InlineResponse20028.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getAssetById"></a>
# **getAssetById**
> InlineResponse2001 getAssetById(id)

Get asset by ID

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let id = "38400000-8cf0-11bd-b23e-10b96e4ef00d"; // String | 

apiInstance.getAssetById(id, (error, data, response) => {
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
 **id** | [**String**](.md)|  | 

### Return type

[**InlineResponse2001**](InlineResponse2001.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getAssetPrice"></a>
# **getAssetPrice**
> InlineResponse20029 getAssetPrice(assetId)

Get the current price of an asset

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let assetId = "38400000-8cf0-11bd-b23e-10b96e4ef00d"; // String | 

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
 **assetId** | [**String**](.md)|  | 

### Return type

[**InlineResponse20029**](InlineResponse20029.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getCandleData"></a>
# **getCandleData**
> InlineResponse20017 getCandleData(orderbook, opts)

Get candlestick data for an orderbook

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderbook = "orderbook_example"; // String | 
let opts = { 
  'start': new Date("2013-10-20T19:20:30+01:00"), // Date | 
  'end': new Date("2013-10-20T19:20:30+01:00"), // Date | 
  'resolution': "resolution_example" // String | 
};
apiInstance.getCandleData(orderbook, opts, (error, data, response) => {
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
 **orderbook** | **String**|  | 
 **start** | **Date**|  | [optional] 
 **end** | **Date**|  | [optional] 
 **resolution** | **String**|  | [optional] 

### Return type

[**InlineResponse20017**](InlineResponse20017.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getCouponsByAssetId"></a>
# **getCouponsByAssetId**
> InlineResponse2002 getCouponsByAssetId(id, opts)

Get coupons for a bond asset

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let id = "38400000-8cf0-11bd-b23e-10b96e4ef00d"; // String | 
let opts = { 
  'start': new Date("2013-10-20T19:20:30+01:00"), // Date | 
  'end': new Date("2013-10-20T19:20:30+01:00"), // Date | 
  'page': 1, // Number | 
  'limit': 100 // Number | 
};
apiInstance.getCouponsByAssetId(id, opts, (error, data, response) => {
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
 **id** | [**String**](.md)|  | 
 **start** | **Date**|  | [optional] 
 **end** | **Date**|  | [optional] 
 **page** | **Number**|  | [optional] [default to 1]
 **limit** | **Number**|  | [optional] [default to 100]

### Return type

[**InlineResponse2002**](InlineResponse2002.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getL1Depth"></a>
# **getL1Depth**
> InlineResponse20012 getL1Depth(orderbookId)

Get the top price levels for a specific orderbook (L1 market depth)

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderbookId = "38400000-8cf0-11bd-b23e-10b96e4ef00d"; // String | 

apiInstance.getL1Depth(orderbookId, (error, data, response) => {
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
 **orderbookId** | [**String**](.md)|  | 

### Return type

[**InlineResponse20012**](InlineResponse20012.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getL2Depth"></a>
# **getL2Depth**
> InlineResponse20011 getL2Depth(orderbookId)

Get the aggregated price levels for a specific orderbook (L2 market depth)

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderbookId = "38400000-8cf0-11bd-b23e-10b96e4ef00d"; // String | 

apiInstance.getL2Depth(orderbookId, (error, data, response) => {
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
 **orderbookId** | [**String**](.md)|  | 

### Return type

[**InlineResponse20011**](InlineResponse20011.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getL3Depth"></a>
# **getL3Depth**
> InlineResponse2006 getL3Depth(orderbookId)

Get all open orders for a specific orderbook (L3 market depth)

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderbookId = "38400000-8cf0-11bd-b23e-10b96e4ef00d"; // String | 

apiInstance.getL3Depth(orderbookId, (error, data, response) => {
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
 **orderbookId** | [**String**](.md)|  | 

### Return type

[**InlineResponse2006**](InlineResponse2006.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getLedgerBalancesSelf"></a>
# **getLedgerBalancesSelf**
> InlineResponse20021 getLedgerBalancesSelf()

Get your own available, locked, and borrowed assets

### Example
```javascript
import {Dora} from 'dora';

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

[**InlineResponse20021**](InlineResponse20021.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getLedgerInterestSelf"></a>
# **getLedgerInterestSelf**
> InlineResponse20023 getLedgerInterestSelf()

Get your own interest

### Example
```javascript
import {Dora} from 'dora';

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

[**InlineResponse20023**](InlineResponse20023.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getLedgerModule"></a>
# **getLedgerModule**
> InlineResponse20018 getLedgerModule()

Get the entire module object, including unborrowed leverage assets and total leverage trackers

### Example
```javascript
import {Dora} from 'dora';

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

[**InlineResponse20018**](InlineResponse20018.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getLedgerModuleByAsset"></a>
# **getLedgerModuleByAsset**
> InlineResponse20019 getLedgerModuleByAsset(assetId)

Get the module object for a single asset ID

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let assetId = "38400000-8cf0-11bd-b23e-10b96e4ef00d"; // String | 

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
 **assetId** | [**String**](.md)|  | 

### Return type

[**InlineResponse20019**](InlineResponse20019.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getLedgerPositionsSelf"></a>
# **getLedgerPositionsSelf**
> InlineResponse20020 getLedgerPositionsSelf()

Get your own positions

### Example
```javascript
import {Dora} from 'dora';

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

[**InlineResponse20020**](InlineResponse20020.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getLedgerValueSelf"></a>
# **getLedgerValueSelf**
> InlineResponse20022 getLedgerValueSelf()

Get your own available, locked, and borrowed USD value; and realized and unrealized PnL

### Example
```javascript
import {Dora} from 'dora';

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

[**InlineResponse20022**](InlineResponse20022.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderById"></a>
# **getOrderById**
> InlineResponse20016 getOrderById(orderId)

Get order by ID

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderId = "38400000-8cf0-11bd-b23e-10b96e4ef00d"; // String | 

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
 **orderId** | [**String**](.md)|  | 

### Return type

[**InlineResponse20016**](InlineResponse20016.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderbookBBO"></a>
# **getOrderbookBBO**
> InlineResponse20012 getOrderbookBBO(orderbookId)

Get the top price levels for a specific orderbook (L1 market depth)

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderbookId = "38400000-8cf0-11bd-b23e-10b96e4ef00d"; // String | 

apiInstance.getOrderbookBBO(orderbookId, (error, data, response) => {
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
 **orderbookId** | [**String**](.md)|  | 

### Return type

[**InlineResponse20012**](InlineResponse20012.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderbookById"></a>
# **getOrderbookById**
> InlineResponse20010 getOrderbookById(orderbookId)

Get orderbook by ID

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderbookId = "38400000-8cf0-11bd-b23e-10b96e4ef00d"; // String | 

apiInstance.getOrderbookById(orderbookId, (error, data, response) => {
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
 **orderbookId** | [**String**](.md)|  | 

### Return type

[**InlineResponse20010**](InlineResponse20010.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderbookDepth"></a>
# **getOrderbookDepth**
> InlineResponse20011 getOrderbookDepth(orderbookId)

Get the aggregated price levels for a specific orderbook (L2 market depth)

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderbookId = "38400000-8cf0-11bd-b23e-10b96e4ef00d"; // String | 

apiInstance.getOrderbookDepth(orderbookId, (error, data, response) => {
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
 **orderbookId** | [**String**](.md)|  | 

### Return type

[**InlineResponse20011**](InlineResponse20011.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderbookOrders"></a>
# **getOrderbookOrders**
> InlineResponse2006 getOrderbookOrders(orderbookId)

Get all open orders for a specific orderbook (L3 market depth)

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderbookId = "38400000-8cf0-11bd-b23e-10b96e4ef00d"; // String | 

apiInstance.getOrderbookOrders(orderbookId, (error, data, response) => {
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
 **orderbookId** | [**String**](.md)|  | 

### Return type

[**InlineResponse2006**](InlineResponse2006.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderbookSummary"></a>
# **getOrderbookSummary**
> InlineResponse20013 getOrderbookSummary(orderbookId)

Get summary of an orderbook

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderbookId = "38400000-8cf0-11bd-b23e-10b96e4ef00d"; // String | 

apiInstance.getOrderbookSummary(orderbookId, (error, data, response) => {
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
 **orderbookId** | [**String**](.md)|  | 

### Return type

[**InlineResponse20013**](InlineResponse20013.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderbookTop"></a>
# **getOrderbookTop**
> InlineResponse20012 getOrderbookTop(orderbookId)

Get the top price levels for a specific orderbook (L1 market depth)

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderbookId = "38400000-8cf0-11bd-b23e-10b96e4ef00d"; // String | 

apiInstance.getOrderbookTop(orderbookId, (error, data, response) => {
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
 **orderbookId** | [**String**](.md)|  | 

### Return type

[**InlineResponse20012**](InlineResponse20012.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getPoolPrice"></a>
# **getPoolPrice**
> InlineResponse20030 getPoolPrice(poolId)

Get the current price of a pool

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let poolId = "38400000-8cf0-11bd-b23e-10b96e4ef00d"; // String | 

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
 **poolId** | [**String**](.md)|  | 

### Return type

[**InlineResponse20030**](InlineResponse20030.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getTradeById"></a>
# **getTradeById**
> InlineResponse20027 getTradeById(tradeId)

Get a trade by ID

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let tradeId = "38400000-8cf0-11bd-b23e-10b96e4ef00d"; // String | 

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
 **tradeId** | [**String**](.md)|  | 

### Return type

[**InlineResponse20027**](InlineResponse20027.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getTrades"></a>
# **getTrades**
> InlineResponse20026 getTrades(opts)

Get a filtered, paginated list of trades

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let opts = { 
  'pools': ["pools_example"], // [String] | 
  'userIds': ["userIds_example"], // [String] | 
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
 **pools** | [**[String]**](String.md)|  | [optional] 
 **userIds** | [**[String]**](String.md)|  | [optional] 
 **start** | **Date**|  | [optional] 
 **end** | **Date**|  | [optional] 
 **page** | **Number**|  | [optional] [default to 1]
 **limit** | **Number**|  | [optional] [default to 100]

### Return type

[**InlineResponse20026**](InlineResponse20026.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getTransactionById"></a>
# **getTransactionById**
> InlineResponse20025 getTransactionById(id)

Get a transaction by ID

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let id = "38400000-8cf0-11bd-b23e-10b96e4ef00d"; // String | 

apiInstance.getTransactionById(id, (error, data, response) => {
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
 **id** | [**String**](.md)|  | 

### Return type

[**InlineResponse20025**](InlineResponse20025.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getTransactions"></a>
# **getTransactions**
> InlineResponse2008 getTransactions(opts)

Get a filtered, paginated list of transactions

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let opts = { 
  'pools': ["pools_example"], // [String] | 
  'userIds': ["userIds_example"], // [String] | 
  'txKinds': ["txKinds_example"], // [String] | 
  'start': new Date("2013-10-20T19:20:30+01:00"), // Date | 
  'end': new Date("2013-10-20T19:20:30+01:00"), // Date | 
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
 **txKinds** | [**[String]**](String.md)|  | [optional] 
 **start** | **Date**|  | [optional] 
 **end** | **Date**|  | [optional] 
 **page** | **Number**|  | [optional] [default to 1]
 **limit** | **Number**|  | [optional] [default to 100]

### Return type

[**InlineResponse2008**](InlineResponse2008.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getUserById"></a>
# **getUserById**
> InlineResponse2003 getUserById(userId)

Get user by ID

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let userId = "38400000-8cf0-11bd-b23e-10b96e4ef00d"; // String | 

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
 **userId** | [**String**](.md)|  | 

### Return type

[**InlineResponse2003**](InlineResponse2003.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getUserLedgerStream"></a>
# **getUserLedgerStream**
> InlineResponse2007 getUserLedgerStream(userId, opts)

Get a snapshot of user&#x27;s ledger updates since a specific time, and opens a stream for further updates

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let userId = "38400000-8cf0-11bd-b23e-10b96e4ef00d"; // String | 
let opts = { 
  'since': new Date("2013-10-20T19:20:30+01:00") // Date | 
};
apiInstance.getUserLedgerStream(userId, opts, (error, data, response) => {
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
 **userId** | [**String**](.md)|  | 
 **since** | **Date**|  | [optional] 

### Return type

[**InlineResponse2007**](InlineResponse2007.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getUserOrdersStream"></a>
# **getUserOrdersStream**
> InlineResponse2006 getUserOrdersStream(userId, orderbookId, opts)

Get a snapshot of user&#x27;s order updates for the given order book since a specific time, and opens a stream for further updates

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let userId = "38400000-8cf0-11bd-b23e-10b96e4ef00d"; // String | 
let orderbookId = "38400000-8cf0-11bd-b23e-10b96e4ef00d"; // String | 
let opts = { 
  'since': new Date("2013-10-20T19:20:30+01:00") // Date | 
};
apiInstance.getUserOrdersStream(userId, orderbookId, opts, (error, data, response) => {
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
 **userId** | [**String**](.md)|  | 
 **orderbookId** | [**String**](.md)|  | 
 **since** | **Date**|  | [optional] 

### Return type

[**InlineResponse2006**](InlineResponse2006.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getUserOrdersStreamAll"></a>
# **getUserOrdersStreamAll**
> InlineResponse2006 getUserOrdersStreamAll(userId, opts)

Get a snapshot of user&#x27;s order updates since a specific time, and opens a stream for further updates

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let userId = "38400000-8cf0-11bd-b23e-10b96e4ef00d"; // String | 
let opts = { 
  'since': new Date("2013-10-20T19:20:30+01:00"), // Date | 
  'orderbookIds': ["orderbookIds_example"] // [String] | 
};
apiInstance.getUserOrdersStreamAll(userId, opts, (error, data, response) => {
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
 **userId** | [**String**](.md)|  | 
 **since** | **Date**|  | [optional] 
 **orderbookIds** | [**[String]**](String.md)|  | [optional] 

### Return type

[**InlineResponse2006**](InlineResponse2006.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getUserSelf"></a>
# **getUserSelf**
> InlineResponse2003 getUserSelf()

Get user details for the authenticated user

### Example
```javascript
import {Dora} from 'dora';

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

[**InlineResponse2003**](InlineResponse2003.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getUserTransactionsStream"></a>
# **getUserTransactionsStream**
> InlineResponse2008 getUserTransactionsStream(userId, opts)

Get a snapshot of user&#x27;s executed transactions since a specific time, and opens a stream for further updates

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let userId = "38400000-8cf0-11bd-b23e-10b96e4ef00d"; // String | 
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
 **userId** | [**String**](.md)|  | 
 **since** | **Date**|  | [optional] 

### Return type

[**InlineResponse2008**](InlineResponse2008.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="ledgerDeposit"></a>
# **ledgerDeposit**
> InlineResponse201 ledgerDeposit(body)

Deposit assets into your account from the outside world

TODO: finish this when implementation has been completed

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let body = new Dora.FundUserRequest(); // FundUserRequest | 

apiInstance.ledgerDeposit(body, (error, data, response) => {
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

### Return type

[**InlineResponse201**](InlineResponse201.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="ledgerWithdraw"></a>
# **ledgerWithdraw**
> InlineResponse201 ledgerWithdraw(body)

Withdraw assets from your account to the outside world

TODO: Finish this when implementation has been completed

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let body = new Dora.FundUserRequest(); // FundUserRequest | 

apiInstance.ledgerWithdraw(body, (error, data, response) => {
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

### Return type

[**InlineResponse201**](InlineResponse201.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageBorrow"></a>
# **leverageBorrow**
> InlineResponse2015 leverageBorrow(body)

Directly borrow assets

TODO: Finish this when implementation has been completed

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let body = null; // Object | 

apiInstance.leverageBorrow(body, (error, data, response) => {
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
 **body** | [**Object**](Object.md)|  | 

### Return type

[**InlineResponse2015**](InlineResponse2015.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageCollateralize"></a>
# **leverageCollateralize**
> InlineResponse2011 leverageCollateralize(body)

Move supplied and available to supplied_collateral and collateral, for a specified position

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let body = new Dora.CollateralizeRequest(); // CollateralizeRequest | 

apiInstance.leverageCollateralize(body, (error, data, response) => {
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
 **body** | [**CollateralizeRequest**](CollateralizeRequest.md)|  | 

### Return type

[**InlineResponse2011**](InlineResponse2011.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageDeCollateralize"></a>
# **leverageDeCollateralize**
> InlineResponse2012 leverageDeCollateralize(body)

Move collateral and supplied_collateral to available and supplied, for a specified position.

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let body = new Dora.DeCollateralizeRequest(); // DeCollateralizeRequest | 

apiInstance.leverageDeCollateralize(body, (error, data, response) => {
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
 **body** | [**DeCollateralizeRequest**](DeCollateralizeRequest.md)|  | 

### Return type

[**InlineResponse2012**](InlineResponse2012.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageIsolateCollateral"></a>
# **leverageIsolateCollateral**
> InlineResponse2016 leverageIsolateCollateral(body)

Create an isolated position by transferring collateral to the position from the user&#x27;s global collateral

### Example
```javascript
import {Dora} from 'dora';

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

[**InlineResponse2016**](InlineResponse2016.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageIsolatePosition"></a>
# **leverageIsolatePosition**
> InlineResponse2017 leverageIsolatePosition(body)

Create an isolated position using all collateral, supplied_collateral, and borrows from the user&#x27;s global position

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let body = new Dora.IsolatePositionRequest(); // IsolatePositionRequest | 

apiInstance.leverageIsolatePosition(body, (error, data, response) => {
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
 **body** | [**IsolatePositionRequest**](IsolatePositionRequest.md)|  | 

### Return type

[**InlineResponse2017**](InlineResponse2017.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageRepay"></a>
# **leverageRepay**
> InlineResponse2015 leverageRepay(body)

Repay borrowed assets

TODO: Finish this when implementation has been completed

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let body = null; // Object | 

apiInstance.leverageRepay(body, (error, data, response) => {
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
 **body** | [**Object**](Object.md)|  | 

### Return type

[**InlineResponse2015**](InlineResponse2015.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageSupply"></a>
# **leverageSupply**
> InlineResponse2013 leverageSupply(body)

Supply leverage for a specific asset

### Example
```javascript
import {Dora} from 'dora';

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

[**InlineResponse2013**](InlineResponse2013.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageUnite"></a>
# **leverageUnite**
> InlineResponse20024 leverageUnite(body)

Combines all isolated positions into a single global position

TODO: Finish this when implementation has been completed

### Example
```javascript
import {Dora} from 'dora';

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

[**InlineResponse20024**](InlineResponse20024.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageWithdraw"></a>
# **leverageWithdraw**
> InlineResponse2014 leverageWithdraw(body)

Withdraw leverage for a specific asset

### Example
```javascript
import {Dora} from 'dora';

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

[**InlineResponse2014**](InlineResponse2014.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="liquidityAdd"></a>
# **liquidityAdd**
> InlineResponse2018 liquidityAdd(body, poolId)

Add liquidity to a pool

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let body = new Dora.LiquidityRequest(); // LiquidityRequest | 
let poolId = "38400000-8cf0-11bd-b23e-10b96e4ef00d"; // String | 

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
 **poolId** | [**String**](.md)|  | 

### Return type

[**InlineResponse2018**](InlineResponse2018.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="liquiditySubtract"></a>
# **liquiditySubtract**
> InlineResponse2018 liquiditySubtract(body, poolId)

Subtract liquidity from a pool

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let body = new Dora.LiquidityRequest(); // LiquidityRequest | 
let poolId = "38400000-8cf0-11bd-b23e-10b96e4ef00d"; // String | 

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
 **poolId** | [**String**](.md)|  | 

### Return type

[**InlineResponse2018**](InlineResponse2018.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="listAssets"></a>
# **listAssets**
> InlineResponse200 listAssets(opts)

List assets

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let opts = { 
  'createdAfter': new Date("2013-10-20T19:20:30+01:00"), // Date | 
  'createdBefore': new Date("2013-10-20T19:20:30+01:00"), // Date | 
  'assetKind': "assetKind_example", // String | Asset kind (BOND, CURRENCY, INTEREST, POOL_SHARE)
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
 **assetKind** | **String**| Asset kind (BOND, CURRENCY, INTEREST, POOL_SHARE) | [optional] 
 **canAddLiquidity** | **Boolean**|  | [optional] 
 **canDirectBorrow** | **Boolean**|  | [optional] 
 **canOnboard** | **Boolean**|  | [optional] 
 **canTrade** | **Boolean**|  | [optional] 
 **canVirtualBorrow** | **Boolean**|  | [optional] 
 **page** | **Number**|  | [optional] [default to 1]
 **limit** | **Number**|  | [optional] [default to 100]

### Return type

[**InlineResponse200**](InlineResponse200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="listOrderBooks"></a>
# **listOrderBooks**
> InlineResponse2009 listOrderBooks(opts)

List order books

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let opts = { 
  'status': "status_example", // String | 
  'baseAssetId': "38400000-8cf0-11bd-b23e-10b96e4ef00d", // String | 
  'quoteAssetId': "38400000-8cf0-11bd-b23e-10b96e4ef00d", // String | 
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
 **status** | **String**|  | [optional] 
 **baseAssetId** | [**String**](.md)|  | [optional] 
 **quoteAssetId** | [**String**](.md)|  | [optional] 
 **page** | **Number**|  | [optional] [default to 1]
 **limit** | **Number**|  | [optional] [default to 100]

### Return type

[**InlineResponse2009**](InlineResponse2009.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="listOrders"></a>
# **listOrders**
> InlineResponse2006 listOrders(opts)

List all orders

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let opts = { 
  'orderbookId': ["orderbookId_example"], // [String] | 
  'kind': "kind_example", // String | 
  'status': "status_example", // String | 
  'side': "side_example", // String | 
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
 **orderbookId** | [**[String]**](String.md)|  | [optional] 
 **kind** | **String**|  | [optional] 
 **status** | **String**|  | [optional] 
 **side** | **String**|  | [optional] 
 **from** | **Date**|  | [optional] 
 **to** | **Date**|  | [optional] 
 **page** | **Number**|  | [optional] [default to 1]
 **limit** | **Number**|  | [optional] [default to 100]

### Return type

[**InlineResponse2006**](InlineResponse2006.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="streamAssetPrices"></a>
# **streamAssetPrices**
> InlineResponse20028 streamAssetPrices(opts)

Get a snapshot of asset prices from a specific date and open a stream for real-time updates

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let opts = { 
  'since': new Date("2013-10-20T19:20:30+01:00") // Date | 
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

### Return type

[**InlineResponse20028**](InlineResponse20028.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="streamCandleData"></a>
# **streamCandleData**
> InlineResponse20017 streamCandleData(orderbook, opts)

Get a snapshot of candlestick data from date provided, and open a stream for real-time updates

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderbook = "orderbook_example"; // String | 
let opts = { 
  'since': new Date("2013-10-20T19:20:30+01:00"), // Date | 
  'resolution': "resolution_example" // String | 
};
apiInstance.streamCandleData(orderbook, opts, (error, data, response) => {
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
 **orderbook** | **String**|  | 
 **since** | **Date**|  | [optional] 
 **resolution** | **String**|  | [optional] 

### Return type

[**InlineResponse20017**](InlineResponse20017.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="streamOrderBookBalances"></a>
# **streamOrderBookBalances**
> InlineResponse20014 streamOrderBookBalances(orderbookId, opts)

Get a snapshot of base and quote balances for an order book and open a stream for real-time updates

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderbookId = "38400000-8cf0-11bd-b23e-10b96e4ef00d"; // String | 
let opts = { 
  'since': new Date("2013-10-20T19:20:30+01:00") // Date | 
};
apiInstance.streamOrderBookBalances(orderbookId, opts, (error, data, response) => {
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
 **orderbookId** | [**String**](.md)|  | 
 **since** | **Date**|  | [optional] 

### Return type

[**InlineResponse20014**](InlineResponse20014.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="streamOrderbookOpenOrders"></a>
# **streamOrderbookOpenOrders**
> InlineResponse2006 streamOrderbookOpenOrders(orderbookId, opts)

Get a snapshot of open orders in an order book and open a stream for real-time updates

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderbookId = "38400000-8cf0-11bd-b23e-10b96e4ef00d"; // String | 
let opts = { 
  'since': new Date("2013-10-20T19:20:30+01:00") // Date | 
};
apiInstance.streamOrderbookOpenOrders(orderbookId, opts, (error, data, response) => {
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
 **orderbookId** | [**String**](.md)|  | 
 **since** | **Date**|  | [optional] 

### Return type

[**InlineResponse2006**](InlineResponse2006.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="streamTrades"></a>
# **streamTrades**
> TradeResponse streamTrades(orderbookId, opts)

Get a snapshot of trades from a specific date and open a stream for real-time updates

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let orderbookId = "38400000-8cf0-11bd-b23e-10b96e4ef00d"; // String | 
let opts = { 
  'since': new Date("2013-10-20T19:20:30+01:00") // Date | 
};
apiInstance.streamTrades(orderbookId, opts, (error, data, response) => {
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
 **orderbookId** | [**String**](.md)|  | 
 **since** | **Date**|  | [optional] 

### Return type

[**TradeResponse**](TradeResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="updateUserConfig"></a>
# **updateUserConfig**
> InlineResponse2005 updateUserConfig(body, userId)

Update user configuration by ID

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let body = new Dora.UpdateUserConfigRequest(); // UpdateUserConfigRequest | 
let userId = "38400000-8cf0-11bd-b23e-10b96e4ef00d"; // String | 

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
 **userId** | [**String**](.md)|  | 

### Return type

[**InlineResponse2005**](InlineResponse2005.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="updateUserConfigSelf"></a>
# **updateUserConfigSelf**
> InlineResponse2005 updateUserConfigSelf(body)

Update user configuration for the authenticated user

### Example
```javascript
import {Dora} from 'dora';

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

[**InlineResponse2005**](InlineResponse2005.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="verifyUser"></a>
# **verifyUser**
> InlineResponse2005 verifyUser(userId)

Verify a user by ID

### Example
```javascript
import {Dora} from 'dora';

let apiInstance = new Dora.DefaultApi();
let userId = "38400000-8cf0-11bd-b23e-10b96e4ef00d"; // String | 

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
 **userId** | [**String**](.md)|  | 

### Return type

[**InlineResponse2005**](InlineResponse2005.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

