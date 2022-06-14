
# IPoolInitializer.sol

    
Creates and initializes V3 Pools

    
*Provides a method for creating and initializing a pool, if necessary, for bundling with other methods that require the pool to exist.*
## Methods
### createAndInitializePoolIfNecessary
```solidity
createAndInitializePoolIfNecessary(address token0, address token1, uint24 fee, uint160 sqrtPriceX96) external payable returns (address pool)
```

            

            
*Provides a method for creating and initializing a pool, if necessary, for bundling with other methods that require the pool to exist.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| token0 | address | The contract address of token0 of the pool |
| token1 | address | The contract address of token1 of the pool |
| fee | uint24 | The fee amount of the v3 pool for the specified token pair |
| sqrtPriceX96 | uint160 | The initial square root price of the pool as a Q64.96 value |

#### Return Values

| Name | Type | Description |
|---|---|---|
| pool | address | Returns the pool address based on the pair of tokens and fee, will return the newly created pool address if necessary |

