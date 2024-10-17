HW1: Explores the Flash Crash of 2010. A constant participation algorithm went rogue, draining liquidity and triggering a market collapse. Simulates how simple random orders impact market dynamics.

HW2: Covers the Parlour Model, explaining how traders balance limit vs market orders based on liquidity. You’ll also learn how trading fees, volatility, and liquidity determine optimal order sizes on different exchanges.

HW3: Dive into limit order book dynamics! Simulate market events to understand how liquidity shapes the order book. Plus, analyze how realized spreads vary across exchanges and impact market maker profitability.

HW4: The Glosten-Milgrom model shows how market makers adjust spreads to defend against informed traders. Learn how bid-ask spreads change based on the risk of adverse selection.

HW5: Kyle’s Model explores how large trades impact prices. Also, what happens when another trader piggybacks on an informed trader’s orders? Spoiler: it dilutes profitability!

HW6: Compare different volatility estimators and see how frequency impacts their accuracy. You’ll also witness the Epps Effect, which shows how stock correlations decrease over shorter time intervals.

HW7: Investigate long memory processes. These models show how past order flow influences future trades. Learn how to forecast market trends using autoregressive models.

HW8: Predict order flow by analyzing how meta orders break into smaller slices. Plus, a deep dive into price manipulation strategies and why certain trade tactics can distort market prices.

HW9: Study Almgren-Chriss and compare optimal trading strategies under different price dynamics. Learn how to balance market impact and risk in real-world trading.

HW10:  Focuses on solving the Fredholm equation numerically using matrix algebra and finding the optimal liquidation strategy in the square-root price impact model. The tasks include deriving matrix expressions, optimizing liquidation strategies across multiple intervals, and



# MTH9879-Market-Microstructure-Models
## Homework Collection: Market Microstructure Models
MTH9879 Market Microstructure Models is a graduate course for students of Baruch MFE Program. All homeworks is done in Jupyter Notebook with R.

The course covers but not limits to the folowing topics:

 - Market mechanisms
 - Theoretical and empirical models of the order book
 - The market/limit order decision
 - Inventory models
 - Rational expectations and models of strategic trading
 - Market making
 - Sequential trade models
 - Understanding the bid-ask spread
 - Variance and covariance estimation
 - The long memory of order flow
 - Models of market impact
 - Market impact of meta-orders
 - Price manipulation
 - Optimal execution strategies
 - Modeling latency
 - Optimal order routing algorithms
 
 
 
### Lecture 1: Market mechanisms and zero intelligence models of the order book
 
 - The limit order book can be viewed as a complex queuing system.
 - Even with very simple rules, complex order flow and price dynamics can be generated.
 - With more realistic rules, zero-intelligence models of the order book can serve as useful tools for comparing the performance of proposed order execution strategies.

 Homework 1 is related to this lecture.
 
 
 
### Lecture 2: Order book and order flow: The market or limit order decision
 
 - Parlour (1998) shows that a rational market order/ limit order decision should depend on the state of the order book
 - Foucault, Kadan and Kandel (2005) model the order book as a market for immediacy, relating the spread to the ratio between patient and impatient traders
 - Rosu (2009) removes many over-stylized features of FKK (2005) by allowing instantaneous cancelation of orders
 - Cont and Kukanov (2013) show how to incorporate the fee structures and current queue lengths in different venues to optimize the market/limit order mix.
 - Bouchaud, Mezard and Potters show that the average order book shape, consistent with ZI simulation and empirical observation, may be derived using a simple price diffusion approximation
Mike and Farmer find a simple empirical relationship between the arrival rates of limit and market orders

Homework 2 is related to this lecture.
 
 
 
### Lecture 3: Inventory models and market-making
 
 - All inventory models have the following characteristics:
    - It is optimal for the market maker to keep inventory close to zero.
    - There will therefore be market impact
       - Market sells cause the price to decrease.
       - Market buys cause the price to increase.
    - The spread is compensation for risk.
       - The spread is increasing in volatility and in the price of risk.

 - In real markets, as in Guilbaud and Pham, as in the case of big tick stocks, the spread is given.
    - A market maker either joins or improves the best quote, or does no business.
 - Market order arrival rates are not symmetric: they depend on the book imbalance.
    - Cartea, Donnelly and Jaimungal solve an optimal control problem to find the optimal placement of limit orders using the book imbalance.

Homework 3 is related to this lecture.



### Lecture 4: Understanding the bid-ask spread

Homework 4 is related to this lecture.



### Lecture 5: Price formation under asymmetric information: The Kyle model

 - In economics, the role of prices is not just to allocate resources efficiently but also to transmit information about the values of assets.
 - The Kyle model exhibits a mechanism through which information may be impounded into market prices.
    - Note however that the market price can depart very substantially from fair value if there is large uninformed demand.
    - If fair value is itself evolving dynamically, the market price may never correspond to fair value.

Homework 5 is related to this lecture.



### Lecture 6: Variance and covariance estimation

 - There has been a huge expansion in the literature on realized variance and covariance estimation since around 2003 with many very interesting papers.
 - As a result, we now have very efficient estimators for realized variance that take into account all of the available information.
    - The newer volatility estimators are all very much more efficient that RV sampled every 5 minutes.
    - Moreover, kernel-based estimators are easily updated in real time by adding the most recent tick and dropping the oldest tick.
 - The article by McAleer and Medeiros is a nice review of the literature up to 2008 or so.
 - The rough volatility forecast seems to be the simplest and bes.

Homework 6 is related to this lecture.



### Lecture 7: Long memory of order flow and market impact

 - Order flow is a long memory process.
    - The dominant effect is order-splitting.
 - Market impact is concave due to selective liquidity taking.
 - Market impact of market orders can be modeled as:
    - Permanent but state-dependent (Lillo)
    - Transient (Bouchaud)
 - Both of these formulations are equivalent.
 - To get quantitative (as opposed to qualitative) agreement with observation, in principle we need to take into account
    - Time-varying liquidity
    - Limit orders and cancelations
 - In practice, it seems (see Taranto) that distinguishing between market orders that change the price and orders that result in no price change is enough for a surprisingly accurate description of market impact.

Homework 7 is related to this lecture.



### Undergraduate Version

The undergraduate version of this course is a series of selected topic in market microstructure and is taught by Prof. Tai-ho Wang at Peking University. This folder contains homeworks and solutions of this course.
