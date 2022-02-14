# stop-loss-eth-yield-farming-trading-bot
Stop-loss ETH yield farming bot

The Farm contract provides functions for entering, exiting, and harvesting rewards from the below protocols.

stop-loss strategy bot is forthcoming to monitor staked token prices.

The bot calls the Farm contract to exit positions when prices are falling. The unstaked tokens are converted to USDC to preserve gains. Currently, the contract uses 1Inch for swaps.

Once prices flatten out, the bot calls the Farm contract to convert USDC back into staking tokens and enter the previously exited staking position.

All staking positions are composed of single ERC20 tokens opposed to liquidity provider (LP) tokens.

The decision to exclude LP token staking was made so that the bot can more easily determine when to exit and enter staking positions. LP token staking would require monitoring impermanent loss--potentially an upgrade for the future.

Here a how to video step by step

https://youtu.be/FDjc0gUEAEM
