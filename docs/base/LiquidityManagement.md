
# LiquidityManagement.sol

    
Liquidity management functions

    
*Internal functions for safely managing liquidity in Uniswap V3*
## Methods
### WETH9
```solidity
WETH9() external view returns (address -)
```

            

            
*Internal functions for safely managing liquidity in Uniswap V3*
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | address | - |

### factory
```solidity
factory() external view returns (address -)
```

            

            
*Internal functions for safely managing liquidity in Uniswap V3*
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | address | - |

### refundETH
```solidity
refundETH() external payable
```

            

            
*Internal functions for safely managing liquidity in Uniswap V3*
### sweepToken
```solidity
sweepToken(address token, uint256 amountMinimum, address recipient) external payable
```

            

            
*Internal functions for safely managing liquidity in Uniswap V3*
#### Parameters

| Name | Type | Description |
|---|---|---|
| token | address | The contract address of the token which will be transferred to `recipient` |
| amountMinimum | uint256 | The minimum amount of token required for a transfer |
| recipient | address | The destination address of the token |

### uniswapV3MintCallback
```solidity
uniswapV3MintCallback(uint256 amount0Owed, uint256 amount1Owed, bytes data) external nonpayable
```

            

            
*Internal functions for safely managing liquidity in Uniswap V3*
#### Parameters

| Name | Type | Description |
|---|---|---|
| amount0Owed | uint256 | The amount of token0 due to the pool for the minted liquidity |
| amount1Owed | uint256 | The amount of token1 due to the pool for the minted liquidity |
| data | bytes | Any data passed through by the caller via the IUniswapV3PoolActions#mint call |

### unwrapWETH9
```solidity
unwrapWETH9(uint256 amountMinimum, address recipient) external payable
```

            

            
*Internal functions for safely managing liquidity in Uniswap V3*
#### Parameters

| Name | Type | Description |
|---|---|---|
| amountMinimum | uint256 | The minimum amount of WETH9 to unwrap |
| recipient | address | The address receiving ETH |


