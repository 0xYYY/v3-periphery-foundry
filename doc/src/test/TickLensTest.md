
# `TickLensTest`

    
Tick Lens contract

    
## Methods
### `getGasCostOfGetPopulatedTicksInWord`
```solidity
function getGasCostOfGetPopulatedTicksInWord(address pool, int16 tickBitmapIndex) external view returns (uint256)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| `pool` | `address` | - |
| `tickBitmapIndex` | `int16` | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `-` | `uint256` | - |

### `getPopulatedTicksInWord`
```solidity
function getPopulatedTicksInWord(address pool, int16 tickBitmapIndex) external view returns ((int24,int128,uint128)[] populatedTicks)
```

            

            
*Get all the tick data for the populated ticks from a word of the tick bitmap of a pool*
#### Parameters

| Name | Type | Description |
|---|---|---|
| `pool` | `address` | The address of the pool for which to fetch populated tick data |
| `tickBitmapIndex` | `int16` | The index of the word in the tick bitmap for which to parse the bitmap and fetch all the populated ticks |

#### Return Values

| Name | Type | Description |
|---|---|---|
| `populatedTicks` | `(int24,int128,uint128)[]` | An array of tick data for the given word in the tick bitmap |


