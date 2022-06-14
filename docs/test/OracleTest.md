
# OracleTest.sol

## Methods
```solidity
consult
```

### Parameters
| Name | Type | Description |
|---|---|---|
| pool | address |  |
| secondsAgo | uint32 |  |


### Return Values
| Name | Type | Description |
|---|---|---|
| arithmeticMeanTick | int24 |  |
| harmonicMeanLiquidity | uint128 |  |

```solidity
getBlockStartingTickAndLiquidity
```

### Parameters
| Name | Type | Description |
|---|---|---|
| pool | address |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | int24 |  |
|  | uint128 |  |

```solidity
getChainedPrice
```

### Parameters
| Name | Type | Description |
|---|---|---|
| tokens | address[] |  |
| ticks | int24[] |  |


### Return Values
| Name | Type | Description |
|---|---|---|
| syntheticTick | int256 |  |

```solidity
getGasCostOfConsult
```

### Parameters
| Name | Type | Description |
|---|---|---|
| pool | address |  |
| period | uint32 |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | uint256 |  |

```solidity
getGasCostOfGetQuoteAtTick
```

### Parameters
| Name | Type | Description |
|---|---|---|
| tick | int24 |  |
| baseAmount | uint128 |  |
| baseToken | address |  |
| quoteToken | address |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | uint256 |  |

```solidity
getOldestObservationSecondsAgo
```

### Parameters
| Name | Type | Description |
|---|---|---|
| pool | address |  |


### Return Values
| Name | Type | Description |
|---|---|---|
| secondsAgo | uint32 |  |
| currentTimestamp | uint32 |  |

```solidity
getQuoteAtTick
```

### Parameters
| Name | Type | Description |
|---|---|---|
| tick | int24 |  |
| baseAmount | uint128 |  |
| baseToken | address |  |
| quoteToken | address |  |


### Return Values
| Name | Type | Description |
|---|---|---|
| quoteAmount | uint256 |  |

```solidity
getWeightedArithmeticMeanTick
```

### Parameters
| Name | Type | Description |
|---|---|---|
| observations | (int24,uint128)[] |  |


### Return Values
| Name | Type | Description |
|---|---|---|
| arithmeticMeanWeightedTick | int24 |  |


### Events

### Errors

