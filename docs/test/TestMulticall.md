
# TestMulticall.sol

    

    
## Methods
### functionThatReturnsTuple
```solidity
functionThatReturnsTuple(uint256 a, uint256 b) external pure returns ((uint256,uint256) tuple)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| a | uint256 | - |
| b | uint256 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| tuple | (uint256,uint256) | - |

### functionThatRevertsWithError
```solidity
functionThatRevertsWithError(string error) external pure
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| error | string | - |

### multicall
```solidity
multicall(bytes[] data) external payable returns (bytes[] results)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| data | bytes[] | The encoded function data for each of the calls to make to this contract |

#### Return Values

| Name | Type | Description |
|---|---|---|
| results | bytes[] | The results from each of the calls passed in via data |

### paid
```solidity
paid() external view returns (uint256 -)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | uint256 | - |

### pays
```solidity
pays() external payable
```

            

            
### returnSender
```solidity
returnSender() external view returns (address -)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | address | - |


