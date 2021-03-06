************************************************
Different Approaches to Model the Bid-Ask Spread
************************************************
This document describes several ways to model bid-ask spreads in asset markets.
Prior literature generated bid-ask spread by endowing a central marketmaker
buying and selling assets to different investors with monopoly power, by
presuming he suffers from adverse selection. Crucially for us, the bid and ask
spread always results from an interaction with at least three types of agents.
In contrast, we allowed traders to set the bid and ask prices themselves. The
reason for basing bid-ask spreads on three traders might be to avoid
indeterminacy of the equilibrium. 

Duffie (OTC Markets)
--------------------
Bid-ask spreads are described via a search model with three participants.
Potential buyers and sellers are randomly matched and bargain about the price
for a trade. The bargaining process is influenced by investors' outside
options. Interestingly, the outcome of this bargaining process is not a bid-ask
spread but only a price, in the same way as it was in the example Joao showed.
The investors are motivated to buy and sell the asset by exogenous shocks.
Besides trading with another investor, a trader might be matched with a
marketmarker. The marketmaker can both buy and sell an asset and can therefore
be considered as having access to an "inventory". The ``Bid`` is the price at
which the marketmaker buys from the seller, and the  ``Ask`` is the price at
which he sells to an investor. Crucially, bid, and ask prices only exists
because of the marketmaker. The analysis in the paper shows that if the
marketmaker has zero bargaining power, the bid-ask spread collapses to zero.
Similarly, if the direct meeting technology between investors improves, the
bid-ask spread falls. 

Gloston and Milgrom
-------------------
While the bid-ask spread in the paper of Duffie et al was explained by a
marketmaker's bargaining power, Gloston and Milgrom explain the spread through
asymmetric information. The spread is necessary for a uniformed marketmaker to
just break even in the face of trading with superior informed traders. Gloson
and Milgrom postulate a model with two types of agents: (Potentially)informed
traders and uniformed marketmakers. The agents trade a (stochastic) asset which
yields a payout in the future. Traders have private information about the final
payout, but also have idiosyncratic liquidity motives for trading. Marketmaker
hold inventory over the asset, do not have private information about the asset
but can discern the trader's valuation from their decision to buy or sell an
asset. The marketmaker can set a bid and ask price. Note, that in Gloston and
Milgrom's paper, Bid and Ask prices are reversed: The bid price is the price at
which the marketmaker is willing to buy an asset, and the ask price is the
price at which he is willing to sell. Thus, ask prices exceeds bids. The bid
price is then set to be the marketmakers valuation of the asset conditional on
the trader wanting the sell the asset: Suppose so far, the marketmaker thinks
the valuation of the asset is $V$, and the markemaker would be willing to buy
the asset at $P=V$. If the next trader however were to sell the asset at that
price, the markemaker might be tempted to revise his valuation of the asset
downwards. Thus, the bid price equals the markemakers valuation of the asset
conditional on the next traders electing to sell the asset. In contrast, the
ask price equals the markemakers valuation of the asset conditional on the next
traders electing to buy the asset.


Glosten: (Electronic Limit Order Book)
--------------------------------------
This is a very interesting extension of his older paper with Milgrom. Glosten
allows traders a larger action space: The investor can not only decide whether
to buy or sell at a given bid and ask but also how much. Suppliers of bids and
asks therefore find it optimal to provide a schedule of bids and asks. The
schedule defines how many asset and liquidity supplier is willing to buy (sell)
at which price. The traders have superior information, they take the schedule
of bids and asks as given, and decide how much to buy and sell to maximize
their expected utility. As in Gloston and Milgrom's paper, the traders are
stochastically allowed to trade, and the liquidity suppliers set the bid and
ask schedules to maximize their expected utility. Bid and Ask prices are again
formed by taking the change in the liquidity providers' valuation for the asset
when the next trader decides to buy or sell an asset into consideration. 

Kyle (1985); Continuous Auction Trading
---------------------------------------
Kyle describes an economy with three types of agents trading a claim to an
asset with publically unknown liquidation value. A trader with private
information about the liquidation value of an asset, a noise trader, and an
uninformed market maker who sets the price to equate supply and demand. The
action spaces of the agents are very interesting: Both the informed and the
uninformed (noise) trade submit market orders, that is they specify the number
of assets they want to trade. However, they do not know the resulting price at
which their orders are fulfilled. The market maker set the price such that his
expectations about the asset's liquidation value, conditional on the sum of the
market orders, equals the price of the asset. Kyle thereby was able to coin a
very influential measurement for the asset's liquidity: Kyle's lambda. Kyle's
lambda specifies how much the price of an asset reacts as a function of the sum
of the market orders. The parameter essentially describes how much the market
maker adjusts his expectations about the asset's liquidation value after
observing the order flow. An illiquid market is said to be characterized by a
high lambda. 

Ho and Stoll (1981)
-------------------
This is an interesting classic paper. The paper derives the bid-ask spread
throguh the utility maximizing behaviour of a single dealer. The dealer has a
personal private opinion about a true value of a asset he trades and is exposed
to random matches with a buyer and a seller of the stock. The likelihood of
matches is influenced by the bid-ask spread set by the dealer. For me, the
paper was similar to the profit maximizing behaviour of a monopolist who takes
the demand curve as give. The optimal bid ask spread equals the optimal bid-ask
spread of a risk-neural deal given the exogenous demand, plus adjustments for
uncertainty in transcation volumne, flucuations of the underlying asset, and
risk preferences.


Comments about Market Structure
-------------------------------
The papers above model the bid-ask spread mostly with dealers. We however have
so far only used traders and not employed dealers. This section describes
traders and dealers in more detail:

Traders can in general trade with two different actions: They can use market
orders or limit orders. Market orders (as used for example in Kyle's paper)
guarantee execution of trade but do not allow the agent to know the price of
the trade in advance. The trade simply states that he/she is willing to trade
and he is then matched with the best available price for him/her. Limit orders
in contrast allow traders to guarantee a price for a trade, but does not allow
traders to guarantee the execution of the trade. The limit order specifies the
highest (lowest) price an agent is willing to buy (sell) and the trade is
executed if another side of the trade can be found willing to offer the sell
(buy) at this or a more favorable price.

Dealers can quote the bid and ask price at which they are willing to trade.
They make their money from buying cheaply and selling expensively. Dealers are
therefore interested in setting the bid and ask spread as widely as possible.
Dealers however compete with public limit orders set by traders (or other
dealers). If the public limit orders are set very aggressively, bid-ask spreads
are small and dealers cannot profit much. In contrast, if spreads are large
dealers benefits handsomely, which however lures other dealers into the market
or encourages public limit orders from traders. 

Most stock markets to me seem to allow both dealers and limit and market
orders. For example, the NYSE is classified as a `hybrid` model, the book says
``[...] the NYSE is essentially an order-driven market, it requires specialist
dealers to offer liquidity if no one else will do so``. Similarly, the LSE has
both a dealer based exchange (SEAQ) and an order book system (SETS). The book
describes markets which are exclusively dealer markets as sports betting market
in which bookmakers act as dealers and the persons betting have no chance to
bet with one another directly but only through the bookmaker. 
