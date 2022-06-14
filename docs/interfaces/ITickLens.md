
# ITickLens.sol
Title: Tick Lens
Details: This avoids the waterfall of fetching the tick bitmap, parsing the bitmap to know which ticks to fetch, and then sending additional multicalls to fetch the tick data
Notice: Provides functions for fetching chunks of tick data for a pool

## Methods
### getPopulatedTicksInWord
```solidity
getPopulatedTicksInWord(address pool, int16 tickBitmapIndex) external view returns ((int24,int128,uint128)[] populatedTicks)
```
Details: This avoids the waterfall of fetching the tick bitmap, parsing the bitmap to know which ticks to fetch, and then sending additional multicalls to fetch the tick data
Notice: Provides functions for fetching chunks of tick data for a pool
#### Parameters

| Name | Type | Description |
|---|---|---|
| pool | address | The address of the pool for which to fetch populated tick data |
| tickBitmapIndex | int16 | The index of the word in the tick bitmap for which to parse the bitmap and fetch all the populated ticks |

#### Return Values

| Type | Description |
|---|---|
(int24,int128,uint128)[] | An array of tick data for the given word in the tick bitmap |


### Events

### Errors

