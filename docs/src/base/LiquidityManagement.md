
# LiquidityManagement.sol

    
Liquidity management functions

    
*Internal functions for safely managing liquidity in Uniswap V3*
## Methods
### WETH9
```solidity
function WETH9() external view returns (address)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | address | - |

### factory
```solidity
function factory() external view returns (address)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | address | - |

### refundETH
```solidity
function refundETH() external payable
```

            
Useful for bundling with mint or increase liquidity that uses ether, or exact output swaps that use ether for the input amount

            
*Refunds any ETH balance held by this contract to the `msg.sender`*
### sweepToken
```solidity
function sweepToken(address token, uint256 amountMinimum, address recipient) external payable
```

            
The amountMinimum parameter prevents malicious contracts from stealing the token from users

            
*Transfers the full amount of a token held by this contract to recipient*
#### Parameters

| Name | Type | Description |
|---|---|---|
| token | address | The contract address of the token which will be transferred to `recipient` |
| amountMinimum | uint256 | The minimum amount of token required for a transfer |
| recipient | address | The destination address of the token |

### uniswapV3MintCallback
```solidity
function uniswapV3MintCallback(uint256 amount0Owed, uint256 amount1Owed, bytes data) external nonpayable
```

            
In the implementation you must pay the pool tokens owed for the minted liquidity. The caller of this method must be checked to be a UniswapV3Pool deployed by the canonical UniswapV3Factory.

            
*Called to `msg.sender` after minting liquidity to a position from IUniswapV3Pool#mint.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| amount0Owed | uint256 | The amount of token0 due to the pool for the minted liquidity |
| amount1Owed | uint256 | The amount of token1 due to the pool for the minted liquidity |
| data | bytes | Any data passed through by the caller via the IUniswapV3PoolActions#mint call |

### unwrapWETH9
```solidity
function unwrapWETH9(uint256 amountMinimum, address recipient) external payable
```

            
The amountMinimum parameter prevents malicious contracts from stealing WETH9 from users.

            
*Unwraps the contract's WETH9 balance and sends it to recipient as ETH.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| amountMinimum | uint256 | The minimum amount of WETH9 to unwrap |
| recipient | address | The address receiving ETH |


