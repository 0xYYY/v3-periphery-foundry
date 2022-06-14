
# Multicall.sol

    
Multicall

    
*Enables calling multiple methods in a single call to the contract*
## Methods
### multicall
```solidity
multicall(bytes[] data) external payable returns (bytes[] results)
```

            

            
*Enables calling multiple methods in a single call to the contract*
#### Parameters

| Name | Type | Description |
|---|---|---|
| data | bytes[] | The encoded function data for each of the calls to make to this contract |

#### Return Values

| Name | Type | Description |
|---|---|---|
| results | bytes[] | The results from each of the calls passed in via data |


