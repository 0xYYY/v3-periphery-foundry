
# LiquidityAmountsTest.sol

    

    
## Methods
### getAmount0ForLiquidity
```solidity
getAmount0ForLiquidity(uint160 sqrtRatioAX96, uint160 sqrtRatioBX96, uint128 liquidity) external pure returns (uint256 amount0)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| sqrtRatioAX96 | uint160 | - |
| sqrtRatioBX96 | uint160 | - |
| liquidity | uint128 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| amount0 | uint256 | - |

### getAmount1ForLiquidity
```solidity
getAmount1ForLiquidity(uint160 sqrtRatioAX96, uint160 sqrtRatioBX96, uint128 liquidity) external pure returns (uint256 amount1)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| sqrtRatioAX96 | uint160 | - |
| sqrtRatioBX96 | uint160 | - |
| liquidity | uint128 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| amount1 | uint256 | - |

### getAmountsForLiquidity
```solidity
getAmountsForLiquidity(uint160 sqrtRatioX96, uint160 sqrtRatioAX96, uint160 sqrtRatioBX96, uint128 liquidity) external pure returns (uint256 amount0, uint256 amount1)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| sqrtRatioX96 | uint160 | - |
| sqrtRatioAX96 | uint160 | - |
| sqrtRatioBX96 | uint160 | - |
| liquidity | uint128 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| amount0 | uint256 | - |
| amount1 | uint256 | - |

### getGasCostOfGetAmount0ForLiquidity
```solidity
getGasCostOfGetAmount0ForLiquidity(uint160 sqrtRatioAX96, uint160 sqrtRatioBX96, uint128 liquidity) external view returns (uint256)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| sqrtRatioAX96 | uint160 | - |
| sqrtRatioBX96 | uint160 | - |
| liquidity | uint128 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
|  | uint256 | - |

### getGasCostOfGetAmount1ForLiquidity
```solidity
getGasCostOfGetAmount1ForLiquidity(uint160 sqrtRatioAX96, uint160 sqrtRatioBX96, uint128 liquidity) external view returns (uint256)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| sqrtRatioAX96 | uint160 | - |
| sqrtRatioBX96 | uint160 | - |
| liquidity | uint128 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
|  | uint256 | - |

### getGasCostOfGetAmountsForLiquidity
```solidity
getGasCostOfGetAmountsForLiquidity(uint160 sqrtRatioX96, uint160 sqrtRatioAX96, uint160 sqrtRatioBX96, uint128 liquidity) external view returns (uint256)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| sqrtRatioX96 | uint160 | - |
| sqrtRatioAX96 | uint160 | - |
| sqrtRatioBX96 | uint160 | - |
| liquidity | uint128 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
|  | uint256 | - |

### getGasCostOfGetLiquidityForAmount0
```solidity
getGasCostOfGetLiquidityForAmount0(uint160 sqrtRatioAX96, uint160 sqrtRatioBX96, uint256 amount0) external view returns (uint256)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| sqrtRatioAX96 | uint160 | - |
| sqrtRatioBX96 | uint160 | - |
| amount0 | uint256 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
|  | uint256 | - |

### getGasCostOfGetLiquidityForAmount1
```solidity
getGasCostOfGetLiquidityForAmount1(uint160 sqrtRatioAX96, uint160 sqrtRatioBX96, uint256 amount1) external view returns (uint256)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| sqrtRatioAX96 | uint160 | - |
| sqrtRatioBX96 | uint160 | - |
| amount1 | uint256 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
|  | uint256 | - |

### getGasCostOfGetLiquidityForAmounts
```solidity
getGasCostOfGetLiquidityForAmounts(uint160 sqrtRatioX96, uint160 sqrtRatioAX96, uint160 sqrtRatioBX96, uint256 amount0, uint256 amount1) external view returns (uint256)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| sqrtRatioX96 | uint160 | - |
| sqrtRatioAX96 | uint160 | - |
| sqrtRatioBX96 | uint160 | - |
| amount0 | uint256 | - |
| amount1 | uint256 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
|  | uint256 | - |

### getLiquidityForAmount0
```solidity
getLiquidityForAmount0(uint160 sqrtRatioAX96, uint160 sqrtRatioBX96, uint256 amount0) external pure returns (uint128 liquidity)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| sqrtRatioAX96 | uint160 | - |
| sqrtRatioBX96 | uint160 | - |
| amount0 | uint256 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| liquidity | uint128 | - |

### getLiquidityForAmount1
```solidity
getLiquidityForAmount1(uint160 sqrtRatioAX96, uint160 sqrtRatioBX96, uint256 amount1) external pure returns (uint128 liquidity)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| sqrtRatioAX96 | uint160 | - |
| sqrtRatioBX96 | uint160 | - |
| amount1 | uint256 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| liquidity | uint128 | - |

### getLiquidityForAmounts
```solidity
getLiquidityForAmounts(uint160 sqrtRatioX96, uint160 sqrtRatioAX96, uint160 sqrtRatioBX96, uint256 amount0, uint256 amount1) external pure returns (uint128 liquidity)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| sqrtRatioX96 | uint160 | - |
| sqrtRatioAX96 | uint160 | - |
| sqrtRatioBX96 | uint160 | - |
| amount0 | uint256 | - |
| amount1 | uint256 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| liquidity | uint128 | - |


