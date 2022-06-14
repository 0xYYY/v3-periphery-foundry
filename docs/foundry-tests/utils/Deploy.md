
# CompleteFixture.sol

## Methods
```solidity
deployCode
```

### Parameters
| Name | Type | Description |
|---|---|---|
| what | string |  |


### Return Values
| Name | Type | Description |
|---|---|---|
| addr | address |  |

```solidity
factory
```

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | address |  |

```solidity
router
```

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | address |  |

```solidity
setUp
```

### Parameters

### Return Values
```solidity
weth9
```

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | address |  |


### Events

### Errors


# SwapRouterFixture.sol

## Methods
```solidity
deployCode
```

### Parameters
| Name | Type | Description |
|---|---|---|
| what | string |  |


### Return Values
| Name | Type | Description |
|---|---|---|
| addr | address |  |

```solidity
factory
```

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | address |  |

```solidity
getBalances
```

### Parameters
| Name | Type | Description |
|---|---|---|
| who | address |  |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | (uint256,uint256,uint256,uint256) |  |

```solidity
router
```

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | address |  |

```solidity
setUp
```

### Parameters

### Return Values
```solidity
weth9
```

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | address |  |


### Events

### Errors


# V3RouterFixture.sol

## Methods
```solidity
deployCode
```

### Parameters
| Name | Type | Description |
|---|---|---|
| what | string |  |


### Return Values
| Name | Type | Description |
|---|---|---|
| addr | address |  |

```solidity
factory
```

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | address |  |

```solidity
router
```

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | address |  |

```solidity
setUp
```

### Parameters

### Return Values
```solidity
weth9
```

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | address |  |


### Events

### Errors


# WETH9.sol

## Methods
```solidity
allowance
```

### Parameters
| Name | Type | Description |
|---|---|---|
| owner | address | The account of the token owner |
| spender | address | The account of the token spender |


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
| spender | address | The account which will be allowed to spend a given amount of the owners tokens |
| amount | uint256 | The amount of tokens allowed to be used by `spender` |


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
| account | address | The account for which to look up the number of tokens it has, i.e. its balance |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | uint256 |  |

```solidity
deposit
```

### Parameters

### Return Values
```solidity
transfer
```

### Parameters
| Name | Type | Description |
|---|---|---|
| recipient | address | The account that will receive the amount transferred |
| amount | uint256 | The number of tokens to send from the sender to the recipient |


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
| sender | address | The account from which the transfer will be initiated |
| recipient | address | The recipient of the transfer |
| amount | uint256 | The amount of the transfer |


### Return Values
| Name | Type | Description |
|---|---|---|
|  | bool |  |


### Events

### Errors

