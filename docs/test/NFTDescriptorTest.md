
# NFTDescriptorTest.sol

## Methods
```solidity
addressToString
```

### Parameters
| Name | Type | Description |
|---|---|---|
| _address | address |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | string |  |

```solidity
constructTokenURI
```

### Parameters
| Name | Type | Description |
|---|---|---|
| params | (uint256,address,address,string,string,uint8,uint8,bool,int24,int24,int24,int24,uint24,address) |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | string |  |

```solidity
feeToPercentString
```

### Parameters
| Name | Type | Description |
|---|---|---|
| fee | uint24 |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | string |  |

```solidity
fixedPointToDecimalString
```

### Parameters
| Name | Type | Description |
|---|---|---|
| sqrtRatioX96 | uint160 |  |
| token0Decimals | uint8 |  |
| token1Decimals | uint8 |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | string |  |

```solidity
generateSVGImage
```

### Parameters
| Name | Type | Description |
|---|---|---|
| params | (uint256,address,address,string,string,uint8,uint8,bool,int24,int24,int24,int24,uint24,address) |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | string |  |

```solidity
getGasCostOfConstructTokenURI
```

### Parameters
| Name | Type | Description |
|---|---|---|
| params | (uint256,address,address,string,string,uint8,uint8,bool,int24,int24,int24,int24,uint24,address) |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | uint256 |  |

```solidity
isRare
```

### Parameters
| Name | Type | Description |
|---|---|---|
| tokenId | uint256 |  |
| poolAddress | address |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | bool |  |

```solidity
rangeLocation
```

### Parameters
| Name | Type | Description |
|---|---|---|
| tickLower | int24 |  |
| tickUpper | int24 |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | string |  |
|  | string |  |

```solidity
sliceTokenHex
```

### Parameters
| Name | Type | Description |
|---|---|---|
| token | address |  |
| offset | uint256 |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | uint256 |  |

```solidity
tickToDecimalString
```

### Parameters
| Name | Type | Description |
|---|---|---|
| tick | int24 |  |
| tickSpacing | int24 |  |
| token0Decimals | uint8 |  |
| token1Decimals | uint8 |  |
| flipRatio | bool |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | string |  |

```solidity
tokenToColorHex
```

### Parameters
| Name | Type | Description |
|---|---|---|
| token | address |  |
| offset | uint256 |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | string |  |


### Events

### Errors

