
# NFTDescriptorTest.sol

    

    
## Methods
### addressToString
```solidity
addressToString(address _address) external pure returns (string -)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| _address | address | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | string | - |

### constructTokenURI
```solidity
constructTokenURI((uint256,address,address,string,string,uint8,uint8,bool,int24,int24,int24,int24,uint24,address) params) external pure returns (string -)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| params | (uint256,address,address,string,string,uint8,uint8,bool,int24,int24,int24,int24,uint24,address) | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | string | - |

### feeToPercentString
```solidity
feeToPercentString(uint24 fee) external pure returns (string -)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| fee | uint24 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | string | - |

### fixedPointToDecimalString
```solidity
fixedPointToDecimalString(uint160 sqrtRatioX96, uint8 token0Decimals, uint8 token1Decimals) external pure returns (string -)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| sqrtRatioX96 | uint160 | - |
| token0Decimals | uint8 | - |
| token1Decimals | uint8 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | string | - |

### generateSVGImage
```solidity
generateSVGImage((uint256,address,address,string,string,uint8,uint8,bool,int24,int24,int24,int24,uint24,address) params) external pure returns (string -)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| params | (uint256,address,address,string,string,uint8,uint8,bool,int24,int24,int24,int24,uint24,address) | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | string | - |

### getGasCostOfConstructTokenURI
```solidity
getGasCostOfConstructTokenURI((uint256,address,address,string,string,uint8,uint8,bool,int24,int24,int24,int24,uint24,address) params) external view returns (uint256 -)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| params | (uint256,address,address,string,string,uint8,uint8,bool,int24,int24,int24,int24,uint24,address) | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | uint256 | - |

### isRare
```solidity
isRare(uint256 tokenId, address poolAddress) external pure returns (bool -)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| tokenId | uint256 | - |
| poolAddress | address | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | bool | - |

### rangeLocation
```solidity
rangeLocation(int24 tickLower, int24 tickUpper) external pure returns (string -, string -)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| tickLower | int24 | - |
| tickUpper | int24 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | string | - |
| - | string | - |

### sliceTokenHex
```solidity
sliceTokenHex(address token, uint256 offset) external pure returns (uint256 -)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| token | address | - |
| offset | uint256 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | uint256 | - |

### tickToDecimalString
```solidity
tickToDecimalString(int24 tick, int24 tickSpacing, uint8 token0Decimals, uint8 token1Decimals, bool flipRatio) external pure returns (string -)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| tick | int24 | - |
| tickSpacing | int24 | - |
| token0Decimals | uint8 | - |
| token1Decimals | uint8 | - |
| flipRatio | bool | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | string | - |

### tokenToColorHex
```solidity
tokenToColorHex(address token, uint256 offset) external pure returns (string -)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| token | address | - |
| offset | uint256 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | string | - |

