
# TestERC20PermitAllowed.sol

## Methods
```solidity
DOMAIN_SEPARATOR
```

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | bytes32 |  |

```solidity
allowance
```

### Parameters
| Name | Type | Description |
|---|---|---|
| owner | address |  |
| spender | address |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | uint256 |  |

```solidity
approve
```

### Parameters
| Name | Type | Description |
|---|---|---|
| spender | address |  |
| amount | uint256 |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | bool |  |

```solidity
balanceOf
```

### Parameters
| Name | Type | Description |
|---|---|---|
| account | address |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | uint256 |  |

```solidity
decimals
```

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | uint8 |  |

```solidity
decreaseAllowance
```

### Parameters
| Name | Type | Description |
|---|---|---|
| spender | address |  |
| subtractedValue | uint256 |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | bool |  |

```solidity
increaseAllowance
```

### Parameters
| Name | Type | Description |
|---|---|---|
| spender | address |  |
| addedValue | uint256 |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | bool |  |

```solidity
name
```

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | string |  |

```solidity
nonces
```

### Parameters
| Name | Type | Description |
|---|---|---|
| owner | address |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | uint256 |  |

```solidity
permit
```

### Parameters
| Name | Type | Description |
|---|---|---|
| holder | address | The address of the token holder, the token owner |
| spender | address | The address of the token spender |
| nonce | uint256 | The holder's nonce, increases at each call to permit |
| expiry | uint256 | The timestamp at which the permit is no longer valid |
| allowed | bool | Boolean that sets approval amount, true for type(uint256).max and false for 0 |
| v | uint8 | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| r | bytes32 | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| s | bytes32 | Must produce valid secp256k1 signature from the holder along with `r` and `v` |


### Return Values
```solidity
permit
```

### Parameters
| Name | Type | Description |
|---|---|---|
| owner | address |  |
| spender | address |  |
| value | uint256 |  |
| deadline | uint256 |  |
| v | uint8 |  |
| r | bytes32 |  |
| s | bytes32 |  |


### Return Values
```solidity
symbol
```

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | string |  |

```solidity
totalSupply
```

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | uint256 |  |

```solidity
transfer
```

### Parameters
| Name | Type | Description |
|---|---|---|
| recipient | address |  |
| amount | uint256 |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | bool |  |

```solidity
transferFrom
```

### Parameters
| Name | Type | Description |
|---|---|---|
| sender | address |  |
| recipient | address |  |
| amount | uint256 |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | bool |  |


### Events

### Errors

