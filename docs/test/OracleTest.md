
# OracleTest.sol

    

    
## Methods
### consult
```solidity
function consult(address pool, uint32 secondsAgo) external view returns (int24 arithmeticMeanTick, uint128 harmonicMeanLiquidity)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| pool | address | - |
| secondsAgo | uint32 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| arithmeticMeanTick | int24 | - |
| harmonicMeanLiquidity | uint128 | - |

### getBlockStartingTickAndLiquidity
```solidity
function getBlockStartingTickAndLiquidity(address pool) external view returns (int24, uint128)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| pool | address | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | int24 | - |
| - | uint128 | - |

### getChainedPrice
```solidity
function getChainedPrice(address[] tokens, int24[] ticks) external view returns (int256 syntheticTick)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| tokens | address[] | - |
| ticks | int24[] | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| syntheticTick | int256 | - |

### getGasCostOfConsult
```solidity
function getGasCostOfConsult(address pool, uint32 period) external view returns (uint256)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| pool | address | - |
| period | uint32 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | uint256 | - |

### getGasCostOfGetQuoteAtTick
```solidity
function getGasCostOfGetQuoteAtTick(int24 tick, uint128 baseAmount, address baseToken, address quoteToken) external view returns (uint256)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| tick | int24 | - |
| baseAmount | uint128 | - |
| baseToken | address | - |
| quoteToken | address | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | uint256 | - |

### getOldestObservationSecondsAgo
```solidity
function getOldestObservationSecondsAgo(address pool) external view returns (uint32 secondsAgo, uint32 currentTimestamp)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| pool | address | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| secondsAgo | uint32 | - |
| currentTimestamp | uint32 | - |

### getQuoteAtTick
```solidity
function getQuoteAtTick(int24 tick, uint128 baseAmount, address baseToken, address quoteToken) external pure returns (uint256 quoteAmount)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| tick | int24 | - |
| baseAmount | uint128 | - |
| baseToken | address | - |
| quoteToken | address | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| quoteAmount | uint256 | - |

### getWeightedArithmeticMeanTick
```solidity
function getWeightedArithmeticMeanTick((int24,uint128)[] observations) external pure returns (int24 arithmeticMeanWeightedTick)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| observations | (int24,uint128)[] | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| arithmeticMeanWeightedTick | int24 | - |


