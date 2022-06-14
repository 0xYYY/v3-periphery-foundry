
# UniswapInterfaceMulticall.sol
Notice: A fork of Multicall2 specifically tailored for the Uniswap Interface

## Methods
### getCurrentBlockTimestamp
```solidity
getCurrentBlockTimestamp() external view returns (uint256 timestamp)
```
Notice: A fork of Multicall2 specifically tailored for the Uniswap Interface
#### Return Values

| Type | Description |
|---|---|
uint256 | - |

### getEthBalance
```solidity
getEthBalance(address addr) external view returns (uint256 balance)
```
Notice: A fork of Multicall2 specifically tailored for the Uniswap Interface
#### Parameters

| Name | Type | Description |
|---|---|---|
| addr | address | - |

#### Return Values

| Type | Description |
|---|---|
uint256 | - |

### multicall
```solidity
multicall((address,uint256,bytes)[] calls) external nonpayable returns (uint256 blockNumber, (bool,uint256,bytes)[] returnData)
```
Notice: A fork of Multicall2 specifically tailored for the Uniswap Interface
#### Parameters

| Name | Type | Description |
|---|---|---|
| calls | (address,uint256,bytes)[] | - |

#### Return Values

| Type | Description |
|---|---|
uint256 | - |
(bool,uint256,bytes)[] | - |


### Events

### Errors

