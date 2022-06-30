
# SwapRouter.sol

    
Uniswap V3 Swap Router

    
*Router for stateless execution of swaps against Uniswap V3*
## Methods
### WETH9
```solidity
function WETH9() external view returns (address)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | address | - |

### exactInput
```solidity
function exactInput((bytes,address,uint256,uint256,uint256) params) external payable returns (uint256 amountOut)
```

            

            
*Swaps `amountIn` of one token for as much as possible of another along the specified path*
#### Parameters

| Name | Type | Description |
|---|---|---|
| params | (bytes,address,uint256,uint256,uint256) | The parameters necessary for the multi-hop swap, encoded as `ExactInputParams` in calldata |

#### Return Values

| Name | Type | Description |
|---|---|---|
| amountOut | uint256 | The amount of the received token |

### exactInputSingle
```solidity
function exactInputSingle((address,address,uint24,address,uint256,uint256,uint256,uint160) params) external payable returns (uint256 amountOut)
```

            

            
*Swaps `amountIn` of one token for as much as possible of another token*
#### Parameters

| Name | Type | Description |
|---|---|---|
| params | (address,address,uint24,address,uint256,uint256,uint256,uint160) | The parameters necessary for the swap, encoded as `ExactInputSingleParams` in calldata |

#### Return Values

| Name | Type | Description |
|---|---|---|
| amountOut | uint256 | The amount of the received token |

### exactOutput
```solidity
function exactOutput((bytes,address,uint256,uint256,uint256) params) external payable returns (uint256 amountIn)
```

            

            
*Swaps as little as possible of one token for `amountOut` of another along the specified path (reversed)*
#### Parameters

| Name | Type | Description |
|---|---|---|
| params | (bytes,address,uint256,uint256,uint256) | The parameters necessary for the multi-hop swap, encoded as `ExactOutputParams` in calldata |

#### Return Values

| Name | Type | Description |
|---|---|---|
| amountIn | uint256 | The amount of the input token |

### exactOutputSingle
```solidity
function exactOutputSingle((address,address,uint24,address,uint256,uint256,uint256,uint160) params) external payable returns (uint256 amountIn)
```

            

            
*Swaps as little as possible of one token for `amountOut` of another token*
#### Parameters

| Name | Type | Description |
|---|---|---|
| params | (address,address,uint24,address,uint256,uint256,uint256,uint160) | The parameters necessary for the swap, encoded as `ExactOutputSingleParams` in calldata |

#### Return Values

| Name | Type | Description |
|---|---|---|
| amountIn | uint256 | The amount of the input token |

### factory
```solidity
function factory() external view returns (address)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | address | - |

### multicall
```solidity
function multicall(bytes[] data) external payable returns (bytes[] results)
```

            
The `msg.value` should not be trusted for any method callable from multicall.

            
*Call multiple functions in the current contract and return the data from all of them if they all succeed*
#### Parameters

| Name | Type | Description |
|---|---|---|
| data | bytes[] | The encoded function data for each of the calls to make to this contract |

#### Return Values

| Name | Type | Description |
|---|---|---|
| results | bytes[] | The results from each of the calls passed in via data |

### refundETH
```solidity
function refundETH() external payable
```

            
Useful for bundling with mint or increase liquidity that uses ether, or exact output swaps that use ether for the input amount

            
*Refunds any ETH balance held by this contract to the `msg.sender`*
### selfPermit
```solidity
function selfPermit(address token, uint256 value, uint256 deadline, uint8 v, bytes32 r, bytes32 s) external payable
```

            
The `owner` is always msg.sender and the `spender` is always address(this).

            
*Permits this contract to spend a given token from `msg.sender`*
#### Parameters

| Name | Type | Description |
|---|---|---|
| token | address | The address of the token spent |
| value | uint256 | The amount that can be spent of token |
| deadline | uint256 | A timestamp, the current blocktime must be less than or equal to this timestamp |
| v | uint8 | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| r | bytes32 | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| s | bytes32 | Must produce valid secp256k1 signature from the holder along with `r` and `v` |

### selfPermitAllowed
```solidity
function selfPermitAllowed(address token, uint256 nonce, uint256 expiry, uint8 v, bytes32 r, bytes32 s) external payable
```

            
The `owner` is always msg.sender and the `spender` is always address(this)

            
*Permits this contract to spend the sender's tokens for permit signatures that have the `allowed` parameter*
#### Parameters

| Name | Type | Description |
|---|---|---|
| token | address | The address of the token spent |
| nonce | uint256 | The current nonce of the owner |
| expiry | uint256 | The timestamp at which the permit is no longer valid |
| v | uint8 | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| r | bytes32 | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| s | bytes32 | Must produce valid secp256k1 signature from the holder along with `r` and `v` |

### selfPermitAllowedIfNecessary
```solidity
function selfPermitAllowedIfNecessary(address token, uint256 nonce, uint256 expiry, uint8 v, bytes32 r, bytes32 s) external payable
```

            
The `owner` is always msg.sender and the `spender` is always address(this) Can be used instead of #selfPermitAllowed to prevent calls from failing due to a frontrun of a call to #selfPermitAllowed.

            
*Permits this contract to spend the sender's tokens for permit signatures that have the `allowed` parameter*
#### Parameters

| Name | Type | Description |
|---|---|---|
| token | address | The address of the token spent |
| nonce | uint256 | The current nonce of the owner |
| expiry | uint256 | The timestamp at which the permit is no longer valid |
| v | uint8 | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| r | bytes32 | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| s | bytes32 | Must produce valid secp256k1 signature from the holder along with `r` and `v` |

### selfPermitIfNecessary
```solidity
function selfPermitIfNecessary(address token, uint256 value, uint256 deadline, uint8 v, bytes32 r, bytes32 s) external payable
```

            
The `owner` is always msg.sender and the `spender` is always address(this). Can be used instead of #selfPermit to prevent calls from failing due to a frontrun of a call to #selfPermit

            
*Permits this contract to spend a given token from `msg.sender`*
#### Parameters

| Name | Type | Description |
|---|---|---|
| token | address | The address of the token spent |
| value | uint256 | The amount that can be spent of token |
| deadline | uint256 | A timestamp, the current blocktime must be less than or equal to this timestamp |
| v | uint8 | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| r | bytes32 | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| s | bytes32 | Must produce valid secp256k1 signature from the holder along with `r` and `v` |

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

### sweepTokenWithFee
```solidity
function sweepTokenWithFee(address token, uint256 amountMinimum, address recipient, uint256 feeBips, address feeRecipient) external payable
```

            
The amountMinimum parameter prevents malicious contracts from stealing the token from users

            
*Transfers the full amount of a token held by this contract to recipient, with a percentage between 0 (exclusive) and 1 (inclusive) going to feeRecipient*
#### Parameters

| Name | Type | Description |
|---|---|---|
| token | address | - |
| amountMinimum | uint256 | - |
| recipient | address | - |
| feeBips | uint256 | - |
| feeRecipient | address | - |

### uniswapV3SwapCallback
```solidity
function uniswapV3SwapCallback(int256 amount0Delta, int256 amount1Delta, bytes _data) external nonpayable
```

            
In the implementation you must pay the pool tokens owed for the swap. The caller of this method must be checked to be a UniswapV3Pool deployed by the canonical UniswapV3Factory. amount0Delta and amount1Delta can both be 0 if no tokens were swapped.

            
*Called to `msg.sender` after executing a swap via IUniswapV3Pool#swap.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| amount0Delta | int256 | The amount of token0 that was sent (negative) or must be received (positive) by the pool by the end of the swap. If positive, the callback must send that amount of token0 to the pool. |
| amount1Delta | int256 | The amount of token1 that was sent (negative) or must be received (positive) by the pool by the end of the swap. If positive, the callback must send that amount of token1 to the pool. |
| _data | bytes | - |

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

### unwrapWETH9WithFee
```solidity
function unwrapWETH9WithFee(uint256 amountMinimum, address recipient, uint256 feeBips, address feeRecipient) external payable
```

            
The amountMinimum parameter prevents malicious contracts from stealing WETH9 from users.

            
*Unwraps the contract's WETH9 balance and sends it to recipient as ETH, with a percentage between 0 (exclusive), and 1 (inclusive) going to feeRecipient*
#### Parameters

| Name | Type | Description |
|---|---|---|
| amountMinimum | uint256 | - |
| recipient | address | - |
| feeBips | uint256 | - |
| feeRecipient | address | - |


