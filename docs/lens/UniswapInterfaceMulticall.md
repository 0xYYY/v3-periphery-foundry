
# UniswapInterfaceMulticall.sol
Notice: A fork of Multicall2 specifically tailored for the Uniswap Interface

## Methods
```solidity
getCurrentBlockTimestamp
```
Notice: A fork of Multicall2 specifically tailored for the Uniswap Interface

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
| timestamp | uint256 |  |

```solidity
getEthBalance
```
Notice: A fork of Multicall2 specifically tailored for the Uniswap Interface

### Parameters
| Name | Type | Description |
|---|---|---|
| addr | address |  |


### Return Values
| Name | Type | Description |
|---|---|---|
| balance | uint256 |  |

```solidity
multicall
```
Notice: A fork of Multicall2 specifically tailored for the Uniswap Interface

### Parameters
| Name | Type | Description |
|---|---|---|
| calls | (address,uint256,bytes)[] |  |


### Return Values
| Name | Type | Description |
|---|---|---|
| blockNumber | uint256 |  |
| returnData | (bool,uint256,bytes)[] |  |


### Events

### Errors

