
# OracleTest.sol

## Methods
### consult
```solidity
consult(address pool, uint32 secondsAgo) external view returns (int24 arithmeticMeanTick, uint128 harmonicMeanLiquidity)
```
#### Parameters

| Name | Type | Description |
|---|---|---|
| pool | address | - |
| secondsAgo | uint32 | - |

#### Return Values

| Type | Description |
|---|---|
int24 | - |
uint128 | - |

### getBlockStartingTickAndLiquidity
```solidity
getBlockStartingTickAndLiquidity(address pool) external view returns (int24, uint128)
```
#### Parameters

| Name | Type | Description |
|---|---|---|
| pool | address | - |

#### Return Values

| Type | Description |
|---|---|
int24 | - |
uint128 | - |

### getChainedPrice
```solidity
getChainedPrice(address[] tokens, int24[] ticks) external view returns (int256 syntheticTick)
```
#### Parameters

| Name | Type | Description |
|---|---|---|
| tokens | address[] | - |
| ticks | int24[] | - |

#### Return Values

| Type | Description |
|---|---|
int256 | - |

### getGasCostOfConsult
```solidity
getGasCostOfConsult(address pool, uint32 period) external view returns (uint256)
```
#### Parameters

| Name | Type | Description |
|---|---|---|
| pool | address | - |
| period | uint32 | - |

#### Return Values

| Type | Description |
|---|---|
uint256 | - |

### getGasCostOfGetQuoteAtTick
```solidity
getGasCostOfGetQuoteAtTick(int24 tick, uint128 baseAmount, address baseToken, address quoteToken) external view returns (uint256)
```
#### Parameters

| Name | Type | Description |
|---|---|---|
| tick | int24 | - |
| baseAmount | uint128 | - |
| baseToken | address | - |
| quoteToken | address | - |

#### Return Values

| Type | Description |
|---|---|
uint256 | - |

### getOldestObservationSecondsAgo
```solidity
getOldestObservationSecondsAgo(address pool) external view returns (uint32 secondsAgo, uint32 currentTimestamp)
```
#### Parameters

| Name | Type | Description |
|---|---|---|
| pool | address | - |

#### Return Values

| Type | Description |
|---|---|
uint32 | - |
uint32 | - |

### getQuoteAtTick
```solidity
getQuoteAtTick(int24 tick, uint128 baseAmount, address baseToken, address quoteToken) external pure returns (uint256 quoteAmount)
```
#### Parameters

| Name | Type | Description |
|---|---|---|
| tick | int24 | - |
| baseAmount | uint128 | - |
| baseToken | address | - |
| quoteToken | address | - |

#### Return Values

| Type | Description |
|---|---|
uint256 | - |

### getWeightedArithmeticMeanTick
```solidity
getWeightedArithmeticMeanTick((int24,uint128)[] observations) external pure returns (int24 arithmeticMeanWeightedTick)
```
#### Parameters

| Name | Type | Description |
|---|---|---|
| observations | (int24,uint128)[] | - |

#### Return Values

| Type | Description |
|---|---|
int24 | - |


### Events

### Errors

