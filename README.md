# Flama Pre-Roadmap 2021

Flama is currently rebuilding the website in https://flama.app. This website will include a dashboard with the 3 first dapps:

# Staking
Flama Staking Shares (FSS) allows users to enjoy FLAMA and FLAPP dividends through staking.

Code: https://github.com/FlamaToken/Staking

# Exchange
Flama Exchange  is a modified Uniswap fork. Trading and flash loans have a 0.35% fee.
Flama Exchange rewards:
- 0.25% of trading fees to Liquidity Providers.
- 0.1% to Flama Staking Shares (FSS) holders. 

FSS distributes fees in FLAPP. The 0.1% feeTo is sent to a FlappFeeConverter smartcontract in F
Uni tokens are converted to FLAP and sent to FSS smartcontract to be distributed among holders, creating a demand for FLAP tokens.
A protocol-wide charge of 0.1% per trade will take effect. This represents 2/7th (28.57%) of the 0.35% fee. Rather than calculating this charge on swaps, which would significantly increase gas costs for all users, the charge is instead calculated when liquidity is added or removed.
The feeTo recipient of the 0.1% charge is a smartcontract (FlappFeeConverter).
“FlappFeeConverter” converts FL (Flama Liquidity Tokens) to FLAPP (FLAP) through the Flama-Exchange or others decentralized exchanges and distributes these FLAPP to the Flama Staking Shares (FSS) smartcontract through another smartcontract called “FlappFeeDistributor”.

# Lending (+ negative interest feature)
We are building a protocol that will allow borrowers to pay negative interest on their loans thanks to farming/staking.
How can we achieve that? Let’s see that with an example:
# Current methods:
Alice deposits 100 coins in a platform to borrow 100 USD with a 5% interest rate.
After 1 year, Alice will have to deposit back the amount borrowed (100 USD) + 5% (5 USD) = 105 USD in order to claim back her 100 coins.
With current borrowing methods, Alice pays 1.05 USD (= 105/100) to claim each coin.

# The inverse lending method:
Alice deposits 100 coins in a platform to borrow 100 USD with a 5% interest rate.
The 100 coins Alice deposited are sent to the highest yield paying farming/staking protocol.
# Option 1 - Collateral-currency yield
The 100 "coins" are sent to a protocol that pays the yield in the same "coins" as the collateral (deposited).
After 1 year, Alice's collateral has grown from 100 to 110 "coins".
Alice will have to deposit 105 USD to claim 110 coins.
With this new method, Alice pays 0,9545 USD (= 105/110) to claim each coin.

# Option 2 - Borrow-currency yield
The 100 "coins" are sent to a protocol that pays the yield in the same "coins" as the borrowed (withdrawn).
After 1 year, Alice's withdrawn amount + interest has been reduced (repayed) from 105 USD to 95 USD.
Alice will have to deposit 95 USD to claim 110 coins.
With this new method, Alice pays 0,95 USD (= 95/100) to claim each coin.

# Option 3 - Different-currency yield
If there's a protocol that pays a higher yield in a different type of curreny, Alice can choose to convert it to either the Collateral or Borrow currency and enjoy the same advantages of options 1 and 2

Now Alice can borrow money without missing on the cost of opportunity of farming/staking!


# Development
You can follow our development at https://github.com/flamatoken

# Contact 
-https://t.me/flamatoken
-https://twitter.com/flamatoken
-https://medium.com/@FLAMATEAM
-https://flamanet.io/
-https://flapptoken.io/ 
