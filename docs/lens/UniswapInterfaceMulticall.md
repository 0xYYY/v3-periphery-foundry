
# UniswapInterfaceMulticall.sol

    

    
*A fork of Multicall2 specifically tailored for the Uniswap Interface*
## Methods
### getCurrentBlockTimestamp
```solidity
getCurrentBlockTimestamp() external view returns (uint256 timestamp)
```

            

            
*A fork of Multicall2 specifically tailored for the Uniswap Interface*
#### Return Values

| Name | Type | Description |
|---|---|---|
| timestamp | uint256 | - |

### getEthBalance
```solidity
getEthBalance(address addr) external view returns (uint256 balance)
```

            

            
*A fork of Multicall2 specifically tailored for the Uniswap Interface*
#### Parameters

| Name | Type | Description |
|---|---|---|
| addr | address | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| balance | uint256 | - |

### multicall
```solidity
multicall((address,uint256,bytes)[] calls) external nonpayable returns (uint256 blockNumber, (bool,uint256,bytes)[] returnData)
```

            

            
*A fork of Multicall2 specifically tailored for the Uniswap Interface*
#### Parameters

| Name | Type | Description |
|---|---|---|
| calls | (address,uint256,bytes)[] | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| blockNumber | uint256 | - |
| returnData | (bool,uint256,bytes)[] | - |


