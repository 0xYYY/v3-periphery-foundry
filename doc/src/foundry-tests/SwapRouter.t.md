
# `ExactInput`

    

    
## Methods
### `createPool`
```solidity
function createPool(address tokenAddressA, address tokenAddressB) external nonpayable
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `tokenAddressA` | `address` | - |
| `tokenAddressB` | `address` | - |

### `deployCode`
```solidity
function deployCode(string what) external nonpayable returns (address addr)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `what` | `string` | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `addr` | `address` | - |

### `exactInput`
```solidity
function exactInput(address[] tokens, uint256 amountIn, uint256 amountOutMinimum) external nonpayable
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `tokens` | `address[]` | - |
| `amountIn` | `uint256` | - |
| `amountOutMinimum` | `uint256` | - |

### `factory`
```solidity
function factory() external view returns (address)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `address` | - |

### `getBalances`
```solidity
function getBalances(address who) external nonpayable returns ((uint256,uint256,uint256,uint256))
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `who` | `address` | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `(uint256,uint256,uint256,uint256)` | - |

### `router`
```solidity
function router() external view returns (address)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `address` | - |

### `setUp`
```solidity
function setUp() external nonpayable
```

            

            
### `weth9`
```solidity
function weth9() external view returns (address)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `address` | - |



# `MultiPool`

    

    
## Methods
### `createPool`
```solidity
function createPool(address tokenAddressA, address tokenAddressB) external nonpayable
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `tokenAddressA` | `address` | - |
| `tokenAddressB` | `address` | - |

### `deployCode`
```solidity
function deployCode(string what) external nonpayable returns (address addr)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `what` | `string` | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `addr` | `address` | - |

### `exactInput`
```solidity
function exactInput(address[] tokens, uint256 amountIn, uint256 amountOutMinimum) external nonpayable
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `tokens` | `address[]` | - |
| `amountIn` | `uint256` | - |
| `amountOutMinimum` | `uint256` | - |

### `factory`
```solidity
function factory() external view returns (address)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `address` | - |

### `getBalances`
```solidity
function getBalances(address who) external nonpayable returns ((uint256,uint256,uint256,uint256))
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `who` | `address` | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `(uint256,uint256,uint256,uint256)` | - |

### `router`
```solidity
function router() external view returns (address)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `address` | - |

### `setUp`
```solidity
function setUp() external nonpayable
```

            

            
### `testEvents`
```solidity
function testEvents() external nonpayable
```

            

            
### `testTwoToOneToZero`
```solidity
function testTwoToOneToZero() external nonpayable
```

            

            
### `testZeroToOneToTwo`
```solidity
function testZeroToOneToTwo() external nonpayable
```

            

            
### `weth9`
```solidity
function weth9() external view returns (address)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `address` | - |

### Events
### `Transfer`
```solidity
event Transfer(address from, address to, uint256 amount)
```

            

            
#### Parameters

| Name | Type | Indexed | Description |
|---|---|---|---|
| `from` | `address` |`true`| - |
| `to` | `address` |`true`| - |
| `amount` | `uint256` |`false`| - |



# `SinglePool`

    

    
## Methods
### `createPool`
```solidity
function createPool(address tokenAddressA, address tokenAddressB) external nonpayable
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `tokenAddressA` | `address` | - |
| `tokenAddressB` | `address` | - |

### `deployCode`
```solidity
function deployCode(string what) external nonpayable returns (address addr)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `what` | `string` | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `addr` | `address` | - |

### `exactInput`
```solidity
function exactInput(address[] tokens, uint256 amountIn, uint256 amountOutMinimum) external nonpayable
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `tokens` | `address[]` | - |
| `amountIn` | `uint256` | - |
| `amountOutMinimum` | `uint256` | - |

### `factory`
```solidity
function factory() external view returns (address)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `address` | - |

### `getBalances`
```solidity
function getBalances(address who) external nonpayable returns ((uint256,uint256,uint256,uint256))
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `who` | `address` | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `(uint256,uint256,uint256,uint256)` | - |

### `router`
```solidity
function router() external view returns (address)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `address` | - |

### `setUp`
```solidity
function setUp() external nonpayable
```

            

            
### `testOneToZero`
```solidity
function testOneToZero() external nonpayable
```

            

            
### `testZeroToOne`
```solidity
function testZeroToOne() external nonpayable
```

            

            
### `weth9`
```solidity
function weth9() external view returns (address)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `address` | - |



# `Swaps`

    

    
## Methods
### `createPool`
```solidity
function createPool(address tokenAddressA, address tokenAddressB) external nonpayable
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `tokenAddressA` | `address` | - |
| `tokenAddressB` | `address` | - |

### `deployCode`
```solidity
function deployCode(string what) external nonpayable returns (address addr)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `what` | `string` | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `addr` | `address` | - |

### `factory`
```solidity
function factory() external view returns (address)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `address` | - |

### `getBalances`
```solidity
function getBalances(address who) external nonpayable returns ((uint256,uint256,uint256,uint256))
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `who` | `address` | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `(uint256,uint256,uint256,uint256)` | - |

### `router`
```solidity
function router() external view returns (address)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `address` | - |

### `setUp`
```solidity
function setUp() external nonpayable
```

            

            
### `weth9`
```solidity
function weth9() external view returns (address)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `address` | - |


