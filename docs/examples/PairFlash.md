
# PairFlash.sol

    
Flash contract implementation

    
*An example contract using the Uniswap V3 flash function*
## Methods
### WETH9
```solidity
WETH9() external view returns (address)
```

            

            
*An example contract using the Uniswap V3 flash function*
#### Return Values

| Name | Type | Description |
|---|---|---|
|  | address | - |

### factory
```solidity
factory() external view returns (address)
```

            

            
*An example contract using the Uniswap V3 flash function*
#### Return Values

| Name | Type | Description |
|---|---|---|
|  | address | - |

### initFlash
```solidity
initFlash((address,address,uint24,uint256,uint256,uint24,uint24) params) external nonpayable
```

            

            
*An example contract using the Uniswap V3 flash function*
#### Parameters

| Name | Type | Description |
|---|---|---|
| params | (address,address,uint24,uint256,uint256,uint24,uint24) | The parameters necessary for flash and the callback, passed in as FlashParams |

### refundETH
```solidity
refundETH() external payable
```

            

            
*An example contract using the Uniswap V3 flash function*
### swapRouter
```solidity
swapRouter() external view returns (address)
```

            

            
*An example contract using the Uniswap V3 flash function*
#### Return Values

| Name | Type | Description |
|---|---|---|
|  | address | - |

### sweepToken
```solidity
sweepToken(address token, uint256 amountMinimum, address recipient) external payable
```

            

            
*An example contract using the Uniswap V3 flash function*
#### Parameters

| Name | Type | Description |
|---|---|---|
| token | address | The contract address of the token which will be transferred to `recipient` |
| amountMinimum | uint256 | The minimum amount of token required for a transfer |
| recipient | address | The destination address of the token |

### uniswapV3FlashCallback
```solidity
uniswapV3FlashCallback(uint256 fee0, uint256 fee1, bytes data) external nonpayable
```

            

            
*An example contract using the Uniswap V3 flash function*
#### Parameters

| Name | Type | Description |
|---|---|---|
| fee0 | uint256 | The fee from calling flash for token0 |
| fee1 | uint256 | The fee from calling flash for token1 |
| data | bytes | The data needed in the callback passed as FlashCallbackData from `initFlash` |

### unwrapWETH9
```solidity
unwrapWETH9(uint256 amountMinimum, address recipient) external payable
```

            

            
*An example contract using the Uniswap V3 flash function*
#### Parameters

| Name | Type | Description |
|---|---|---|
| amountMinimum | uint256 | The minimum amount of WETH9 to unwrap |
| recipient | address | The address receiving ETH |


