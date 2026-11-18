

<!-- === Source: MinerU_markdown_An_Introduction_to_the_Mathematics_of_Financial_Derivatives_Solution_Manual_Neftci_1_2122707919320489998.md (Page 1) === -->

## CHAPTER 1

1. (a) Payoff diagram at expiration: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5882bd1f-b733-4ed9-8bdc-4c98ae290af0/41d4673b42f9456b31c05104f1079171471eeaedab7ac9b0444ef0990917bd48.jpg)



FIGURE 0.1 Payoff diagram for both a short sale of stock and an at-the-money call.


Payoff diagram at expiration: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5882bd1f-b733-4ed9-8bdc-4c98ae290af0/b30c57b02b55757531af811b8e4b5e71ff4d418870b67a577c5ceafb679c80e0.jpg)



FIGURE 0.2 Payoff diagram for a long put with strike $K_{1}$ and a long call with strike $K_{2}$ , $K_{1} < K_{2}$ .


Payoff diagram at expiration: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5882bd1f-b733-4ed9-8bdc-4c98ae290af0/f3c6d9e6fbecb29d926a85aaeb207598f7a4fb6b117cc5ec8c00f2b559f28704.jpg)



FIGURE 0.3 Payoff diagram for a (long put/short call) combination at $K_{1}$ plus a (long call/short put) combination at $K_{2} > K_{1}$


(b) Payoff diagram before expiration: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5882bd1f-b733-4ed9-8bdc-4c98ae290af0/50d138fa94b90bc32297611fa6b0587d1f5d591ac07c2db6e4f4f1588eb6ff2c.jpg)



FIGURE 0.4 Pre-maturity payoff diagram for both a short sale of stock and an at-the-money call.


Payoff diagram before expiration: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5882bd1f-b733-4ed9-8bdc-4c98ae290af0/9f176f2696792fea877a60f4af500c72f4e4620dbf6b9571ba8537e09fd01564.jpg)



FIGURE 0.5 Pre-maturity payoff diagram for a long put with strike $K_{1}$ and a long call with strike $K_{2}$ , $K_{1} < K_{2}$ .


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5882bd1f-b733-4ed9-8bdc-4c98ae290af0/4dbe58a8a9531dc9c9afd7b16ab662fe207f03beb038a13f41010e825479075b.jpg)



FIGURE 0.6 Pre-maturity payoff diagram for a (long put/short call) combination at $K_{1}$ plus a (long call/short put) combination at $K_{2} > K_{1}$ .


2. (a) Let $N$ denote the notional amount of the swap and $L_{12}$ and $L_{18}$ the USD Libor rate at 12 months and 18 months respectively. The cash flows are given by 


12 months 18 months 24 months


<table><tr><td>Floating leg</td><td>+N</td><td>+N × <eq>\frac{L_{12}}{2}</eq></td><td>+N × (1 + <eq>\frac{L_{18}}{2}</eq>)</td></tr><tr><td>Fixed leg</td><td>-N</td><td>-N × <eq>\frac{.05}{2}</eq></td><td>-N × (1 + <eq>\frac{.05}{2}</eq>)</td></tr></table>


where the 1 in the 24 months column represents the notional amount. 


(b) If one had a floating rate obligation and wished to pay a fixed rate, $\kappa$ , then enter into two FRA contracts at rate $\kappa$ with maturity 18 and 24 months. For example, at 18 months, if the floating rate were above $\kappa$ , then the FRA would be in-the-money by precisely the amount required to offset the higher floating rate payment. Therefore, the total payment is at the rate $\kappa$ . 

(c) If one had a floating rate obligation and wished to pay a fixed rate, a swap is not necessary as long as the appropriate interest rate options are available. A long position in an interest rate cap at rate $\kappa$ and a short position in an interest rate floor at rate $\kappa$ , both maturing on the floating rate payment date, ensure that a fixed rate of $\kappa$ is paid. If the floating rate, say $r_{T}$ , is above $\kappa$ at expiry, a net payment at rate $\kappa$ is required after taking into account the value of the cap, $N \times (r_{T} - \kappa)$ . If the floating rate is below $\kappa$ at expiry, say $r_{T}$ , then a payment at rate $r_{T}$ must be made on the floating rate obligation. However, the short position in the floor requires an additional payment of $N \times (\kappa - r_{T})$ . The result is a total payment at precisely rate $\kappa$ . 

3. (a) $S_{t}(1 + r) \leq F_{t} \leq (S_{t} + c + s)(1 + r)$ where $c$ is the annual storage cost for 1 ton of wheat, $s$ is the annual insurance cost for 1 ton of wheat, and $r$ is the simple interest rate. If $F_{t} > (S_{t} + c + s)(1 + r)$ , then construct the following arbitrage portfolio 

<table><tr><td>Position</td><td>Payoff at t</td><td>Payoff at T</td></tr><tr><td>Short futures</td><td>0</td><td><eq>F_t - S_T</eq></td></tr><tr><td>Borrow <eq>S_t + c + s</eq></td><td><eq>+(S_t + c + s)</eq></td><td><eq>-(S_t + c + s)(1 + r)</eq></td></tr><tr><td>Buy wheat and pay storage, insurance costs</td><td><eq>-(S_t + c + s)</eq></td><td><eq>S_T</eq></td></tr><tr><td>Total</td><td>0</td><td><eq>F_t - (S_t + c + s)(1 + r) &gt; 0</eq></td></tr></table>

Thus, $F_{t} \leq (S_{t} + c + s)(1 + r)$ . If $F_{t} < (S_{t} + c + s)(1 + r)$ , one cannot immediately reverse the holdings in the above portfolio to create another arbitrage portfolio. A problem arises since wheat is not typically held as an investment asset. If one sells wheat, it is not reasonable to assume that one is entitled to receive the storage and insurance. Therefore, a weaker condition ensues with $F_{t} \geq S_{t}(1 + r)$ but not $F_{t} \geq (S_{t} + c + s)(1 + r)$ . If the asset were of a financial nature or a commodity held for investment such as gold, one could sell the asset and save on the storage and insurance costs. These assets produce an exact relationship, $F_{t} = (S_{t} + c + s)(1 + r)$ . Holding an asset such as wheat has value since it may be consumed. For instance, a large bakery requires wheat for production and maintains an inventory. These companies would be reluctant to substitute a futures contract for the actual underlying. Hence, the price of a futures is allowed to be less than $(S_{t} + c + s)(1 + r)$ . However, if $F_{t} < S_{t}(1 + r)$ , then construct the following arbitrage portfolio 

<table><tr><td>Position</td><td>Payoff at t</td><td>Payoff at T</td></tr><tr><td>Buy futures</td><td>0</td><td><eq>S_T - F_t</eq></td></tr><tr><td>Invest <eq>S_t</eq></td><td><eq>-S_t</eq></td><td><eq>+S_t(1+r)</eq></td></tr><tr><td>Sell wheat</td><td><eq>+S_t</eq></td><td><eq>-S_T</eq></td></tr><tr><td>Total</td><td>0</td><td><eq>S_t(1+r) - F_t &gt; 0</eq></td></tr></table>


Thus, $F_{t} \geq S_{t}(1 + r)$ and combining the two inequalities implies 


$$
S _ {t} (1 + r) \leq F _ {t} \leq (S _ {t} + c + s) (1 + r)
$$

(b) $F_t = \$1,500 < \$1,543.50 = (1,470)(1+.05) = S_t(1+r)$ . This violates the above inequality. To take advantage of this arbitrage opportunity, follow the second arbitrage strategy outlined above. 

(c) Profit / Loss = 1,543.50 - 1,500 = $43.50. 

4. (a) $F_{t} = S_{t}(1 + r)^{(T-t)} = \$105$ where T - t = 1 year. 

(b) $F_{t} = 101$ . Consider the following arbitrage portfolio 

<table><tr><td>Position</td><td>Payoff at t</td><td>Payoff at T</td></tr><tr><td>Long forward</td><td>$0</td><td><eq>S_{T} - \$101</eq></td></tr><tr><td>Short stock</td><td>+\$100</td><td>-<eq>S_{T}</eq></td></tr><tr><td>Invest at risk - free rate</td><td>-\$100</td><td>+\$105</td></tr><tr><td>Total</td><td>$0</td><td>$4</td></tr></table>

or the following arbitrage portfolio 

<table><tr><td>Position</td><td>Payoff at t</td><td>Payoff at T</td></tr><tr><td>Short stock</td><td>+$100</td><td><eq>-S_{T}</eq></td></tr><tr><td>Long Call</td><td>-$3.0</td><td><eq>\max(S_{T} - \$100, 0)</eq></td></tr><tr><td>Short Put</td><td>+$3.5</td><td><eq>\min(S_{T} - \$100, 0)</eq></td></tr><tr><td>Invest PV(100) at risk - free rate</td><td>-<eq>\frac{100}{1.05}</eq></td><td>$100</td></tr><tr><td>Total</td><td>$5.26</td><td>$0</td></tr></table>

## CHAPTER 2

1. (a) $p^{*} = \frac{r - d}{u - d} = \frac{1 + .05\Delta - \frac{260}{280}}{\frac{320}{280} - \frac{260}{280}} = .3917$ 

(b) Value of the call option. 

$$
\begin{array}{r c l} C _ {t} & = & \frac {1}{(1 + . 0 5 \Delta)} E _ {\tilde {p}} (C _ {t + \Delta}) \\ & = & \frac {1}{(1 + . 0 5 \Delta)} (3 2 0 - 2 8 0) \times p ^ {*} \\ & = & \S 1 5. 4 7 \end{array}
$$

(c) Normalize by $S_{t}$ . The elements of the state price vector must be solved. Consider the following two equations 

$$
\begin{array}{r l r} {1} & {=} & {(1 + r \Delta) \psi_ {u} + (1 + r \Delta) \psi_ {d}} \\ {S _ {t}} & {=} & {S _ {t + 1} ^ {u} \psi_ {u} + S _ {t + 1} ^ {d} \psi_ {d}} \end{array}
$$

and after dividing the second equation by $S_{t}$ 

$$
\begin{array}{r l r} {1} & {=} & {(1 + r \Delta) \psi_ {u} + (1 + r \Delta) \psi_ {d}} \\ {1} & {=} & {\frac {S _ {t + 1} ^ {u}}{S _ {t}} \psi_ {u} + \frac {S _ {t + 1} ^ {d}}{S _ {t}} \psi_ {d}} \end{array}
$$

Substitute in the values for $r$ , $S_{t + 1}^{u}$ , $S_{t + 1}^{d}$ and express these equations as 

$$
\left( \begin{array}{c c} 1. 0 1 2 5 & 1. 0 1 2 5 \\ \frac {3 2 0}{2 8 0} & \frac {2 6 0}{2 8 0} \end{array} \right) \binom{\psi_ {u}}{\psi_ {d}} = \binom{1}{1}
$$

Solving this system gives $\psi_{u} = .3868$ and $\psi_{d} = .6008$ . The first equation 

$$
1 = (1 + r \Delta) \psi_ {u} + (1 + r \Delta) \psi_ {d}
$$

demonstrates that up and down probabilities are calculated as $\tilde{p}^u = (1 + r\Delta)\psi_u = .3917$ and $\tilde{p}^d = 1 - \tilde{p}^u = (1 + r\Delta)\psi_d = .6083$ . Observe that the quantity $\tilde{p}^u$ is the same as $p^*$ in part (a). 

(d) Observe that the discounted stock price is a martingale under the risk - neutral measure calculated by the $S_{t}$ normalization. 

$$
\begin{array}{r c l} E \left[ \frac {S _ {t + 1}}{(1 + r \Delta)} \Bigg | \mathcal {I} _ {t} \right] & = & \frac {1}{(1 + r \Delta)} \left(\tilde {p} ^ {u} \times S _ {t + 1} ^ {u} + \tilde {p} ^ {d} \times S _ {t + 1} ^ {d}\right) \\ & = & \frac {1}{1 . 0 1 2 5} (. 3 9 1 7 \times 3 2 0 +. 6 0 8 3 \times 2 6 0) \\ & = & 2 8 0 \\ & = & S _ {t} \end{array}
$$

(e) Only the up state is relevant for pricing the call option as the call expires worthless if the stock decreases to $260 next period. The call price equals 

$$
C _ {t} = 4 0 \psi_ {u} = 1 5. 4 7
$$

The same price calculated in part (b). 

(f) No, different martingale measures (i.e. different risk neutral probabilities $\tilde{p}^u$ and $\tilde{p}^d$ ) produce different call values. However, an option's fair market value is independent of the procedure used to obtain $\tilde{p}$ (or $p^*$ ). 

(g) A different normalization (numeraire asset) is used. An analogue to part (f) would be a statement asserting that the arbitrage - free option price is independent of the numeraire asset. 

(h) The risk premium incorporated in the option's price satisfies: $(1 + r + \text{risk premium for } C_t) = E^{empirical} \left[ \frac{C_{t+1}}{C_t} \right]$ . This risk premium is usually not calculated in the real world. One uses risk-neutral probabilities for call pricing, $E^{risk neutral} \left[ \frac{C_{t+1}}{C_t} \right] = 1 + r$ and not $E^{empirical} \left[ \frac{C_{t+1}}{C_t} \right]$ . In an incomplete market, there may exist risk premiums which require explicit calculation. 

2. (a) Assume the risk-free interest rate $r$ is zero and consider the system of equations given by 

$$
{\left[ \begin{array}{l l} 1 2 4 & 7 1 \\ 8 3 & 6 1 \\ 9 2 & 1 6 0 \end{array} \right]} {\left[ \begin{array}{l} \psi_ {1} \\ \psi_ {2} \end{array} \right]} = {\left[ \begin{array}{l} A _ {0} \\ B _ {0} \\ C _ {0} \end{array} \right]}
$$

If there exists $\psi_{1}$ and $\psi_{2}$ with the properties 

$$
\begin{array}{l l} 1. & \psi_ {1} + \psi_ {2} = \frac {1}{(1 + r)} = 1 \qquad \text { assumed } r = 0 \\ 2. & \psi_ {1}, \psi_ {2} > 0 \end{array}
$$

such that the right hand side of this system of equations is positive, then the “current prices” are arbitrage - free. In this particular case, since no current prices are specified, there are an infinite number of possible $\psi_{1}$ and $\psi_{2}$ solutions in which both state prices are positive, sum to the discount factor, and generate positive values for $A_{0}$ , $B_{0}$ , and $C_{0}$ . 

(b) If no such solution exists, then at least one of the current prices $(A_{0}, B_{0}, \text{or } C_{0})$ is non-positive. In this case, one would “buy” the asset for the non-positive price and be assured of positive payoffs in all future states of the world. Hence, an arbitrage profit exists. 

(c) Let $\psi_{1} = \psi_{2} = \frac{1}{2}$ . Then, 

$$
{\left[ \begin{array}{l} A _ {0} \\ B _ {0} \\ C _ {0} \end{array} \right]} = {\left[ \begin{array}{l} 9 7. 5 \\ 7 2. 0 \\ 1 2 6. 0 \end{array} \right]}
$$

(d) The futures' strike price for asset B is chosen such that the current value of the contract is worth zero. Thus, $F_0 = 0$ . In this case, given $\psi_1$ , the strike price $K$ satisfies, $K = 22\psi_1 + 61$ . This value of $K$ was generated by the equation 

$$
0 = \psi_ {1} (8 3 - K) + (1 - \psi_ {1}) (6 1 - K)
$$

where $\psi_{1} = \tilde{p}_{1}$ since $r = 0$ . In general, risk-neutral probabilities and not state prices are used. Alternatively, if the contract was struck on a previous date with a previously specified strike price $K$ , it's current value is given by the expected payoff under the risk-neutral measure. 

$$
F _ {0} = \tilde {p} (8 3 - K) + (1 - \tilde {p}) (6 1 - K)
$$

Note that in general one does not discount the payoff when pricing a futures' contract. 

(e) The put option on asset C only depends on the first state as the 92 payoff is less than the strike price. Its price is therefore the discounted payoff in the first state, $P_{0} = (125 - 92)\psi_{1} = 33\psi_{1}$ . For the put option, the state price is used as discounting must be taken into account. 

3. (a) The three equations are captured in the following linear system. 

$$
\left( \begin{array}{c c} S _ {t + \Delta} ^ {u} & S _ {t + \Delta} ^ {d} \\ C _ {t + \Delta} ^ {u} & C _ {t + \Delta} ^ {d} \\ 1 & 1 \end{array} \right) \binom{\psi_ {1}}{\psi_ {2}} = \binom{S _ {t}}{\frac {C _ {t}}{1 + r}}
$$

(b) The two step binomial tree is 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5882bd1f-b733-4ed9-8bdc-4c98ae290af0/1cd0f628f327282a6eaaf78762490429d526351d560d5b0c593d72a6112b79dc.jpg)



FIGURE 0.7 Two step binomial tree for problem 3, part (b)


If the tree were arbitrage - free, one could write three 3 - equation systems for the entire tree, one corresponding to each of the three nodes; $S_{t}$ , $S_{t + \Delta}^{u}$ , and $S_{t + \Delta}^{d}$ . 

(c) The three 3 - equation systems are 

$$
\left( \begin{array}{c c} S _ {t + 2 \Delta} ^ {u u} & S _ {t + 2 \Delta} ^ {u d} \\ C _ {t + 2 \Delta} ^ {u u} & C _ {t + 2 \Delta} ^ {u d} \\ 1 & 1 \end{array} \right) \binom{\psi_ {1} ^ {u}}{\psi_ {2} ^ {u}} = \binom{S _ {t + \Delta} ^ {u}}{C _ {t + \Delta} ^ {u}}
$$

$$
\left( \begin{array}{c c} S _ {t + 2 \Delta} ^ {d u} & S _ {t + 2 \Delta} ^ {d d} \\ C _ {t + 2 \Delta} ^ {d u} & C _ {t + 2 \Delta} ^ {d d} \\ 1 & 1 \end{array} \right) \binom{\psi_ {1} ^ {d}}{\psi_ {2} ^ {d}} = \left( \begin{array}{c} S _ {t + \Delta} ^ {d} \\ C _ {t + \Delta} ^ {d} \\ \frac {1}{1 + r} \end{array} \right)
$$

$$
\left( \begin{array}{c c} S _ {t + \Delta} ^ {u} & S _ {t + \Delta} ^ {d} \\ C _ {t + \Delta} ^ {u} & C _ {t + \Delta} ^ {d} \\ 1 & 1 \end{array} \right) \binom{\psi_ {1}}{\psi_ {2}} = \binom{S _ {t}}{\frac {C _ {t}}{\frac {1}{1 + r}}}
$$

(d) Let $\tau$ be the terminal time. Consistency is the notion that at time zero, all intermediate nodes on the tree are arbitrage - free if the terminal nodes are arbitrage - free. A state price, $\psi_i(t)$ , is the discounted risk - neutral probability of that state occurring, $\psi_i(t) = \frac{p_i(0,t)}{B(t)}$ . Let $p_i(0,t)$ denote the risk - neutral probability that state $i$ occurs at time $t$ given the initial node as the current position. The term $B(t)$ represents the discount factor from 0 to time $t$ , $B(t) = \frac{1}{(1 + r)^t} > 0$ . Since the terminal nodes are arbitrage - free, the values of $\psi_i(\tau)$ satisfy two properties 

(1) 

$$
\begin{array}{l} \psi_ {i} (\tau) > 0 \Rightarrow p _ {i} (0, \tau) > 0 \forall i \\ \sum_ {i} \psi_ {i} (\tau) = \frac {1}{B (\tau)} \end{array}\tag{2}
$$

It remains to show that $\psi_{i}(t)$ also satisfy the same two properties for $0 \leq t \leq \tau$ and all states i which can occur at time t. Note that the number of states depends on t. At time t, the sum extends from i = 1 to $i = 2^{t}$ (non recombining tree). 

Since $p_{i}(0,\tau)>0$ for all i, all intermediate nodes are accessible from the initial node. If an intermediate node was not accessible, $p_{i}(0,t)=0$ , then there would exist a terminal node with $p_{i}(0,\tau)=0$ . This would contradict property (1) above. Therefore, $\psi_{i}(t)>0$ for all i and for all t. 

The second property requires the sum of the state prices across the number of states to equal the discount factor for a fixed $t$ . This assertion follows from 

$$
\begin{array}{r l} & \sum_ {i} p _ {i} (0, t) = 1 \quad \forall t \\ \Rightarrow & B (t) \sum_ {i} \psi_ {i} (t) = 1 \quad \forall t \\ \Rightarrow & \sum_ {i} \psi_ {i} (t) = \frac {1}{B (t)} \quad \forall t \end{array}
$$

Thus, the sum of the state prices across all the states at time $t$ equals the discount factor. Therefore, all intermediate nodes are free of arbitrage. 

4. (a) $u = e^{\sigma \sqrt{\Delta}} \Rightarrow \sigma = \frac{\log(u)}{\sqrt{\Delta}} = .48$ (where $\Delta = \frac{1}{12}$ when annualized). 

(b) Assume that $S_{0} = 50$ and K = 50. The 4-step binomial tree for the stock: 

$$
\begin{array}{c c c c c} t = 0 & t = 1 & t = 2 & t = 3 & t = 4 \\ & & & & 8 7. 4 5 \\ & & & 7 6. 0 4 \\ & & 6 6. 1 3 & & 6 6. 1 3 \\ & 5 7. 5 0 & & 5 7. 5 0 \\ 5 0 & & 5 0 & & 5 0 \\ & 4 3. 4 8 & & 4 3. 4 8 \\ & & 3 7. 8 0 & & 3 7. 8 0 \\ & & & 3 2. 8 8 \\ & & & & 2 8. 5 9 \end{array}
$$

The risk - neutral up probability, $p = \frac{(1 + r\Delta - d)}{(u - d)} = \frac{1 + \frac{05}{12} - .87}{1.15 - .87} = .48$ , is used to find the call premium tree. Work backwards from the terminal node at $t = 4$ where the call premium is simply max ( $S_4 - 100, 0$ ). For example, at $t = 3$ , the top node is priced as $\frac{p \times 37.45 + (1 - p) \times 16.13}{1 + r\Delta} = \$26.25$ . 

$$
\begin{array}{c c c c c} t = 0 & t = 1 & t = 2 & t = 3 & t = 4 \\ & & & & 3 7. 4 5 \\ & & & 2 6. 2 5 \\ & & 1 6. 5 4 & & 1 6. 1 3 \\ & 9. 8 2 & & 7. 7 1 \\ 5. 6 0 & & 3. 6 9 & & 0 \\ & 1. 7 6 & & 0 \\ & & 0 & & 0 \\ & & & 0 \end{array}
$$

(c) $C_0 = \$5.60$ , the initial node on the call premium tree. 

5. (a) $u = e^{(.30)\sqrt{\frac{1}{12}}} = 1.09$ . The binomial tree for the stock is 

$$
\begin{array}{c c c c} t = 0 & t = 1 & t = 2 & t = 3 \\ & & & 1 3 2. 2 6 \\ & & 1 2 1. 3 0 \\ & 1 1 1. 2 3 & & 1 1 1. 2 3 \\ 1 0 2 & & 1 0 2 \\ & 9 3. 5 4 & & 9 3. 5 4 \\ & & 8 5. 7 8 & \\ & & & 7 8. 6 6 \end{array}
$$

while the terminal values for the call option are 

The hedging portfolio one should use to replicate the option payoffs is as follows: Time 0 

<table><tr><td>Position</td><td>Value of Portfolio</td></tr><tr><td>Borrow at the risk - free rate</td><td>-$16.113</td></tr><tr><td>Long 0.173 shares</td><td>+$17.646</td></tr><tr><td>Total Value</td><td>=$1.53</td></tr></table>

## Time 1

- If tick was down, the portfolio is now worth $0, do nothing the rest of the option's life and the portfolio matches the option payoffs since it expires worthless. 

■ If the tick was up, the portfolio is now worth $3.06. Adjust the portfolio in the following way: 

<table><tr><td>Position</td><td>Value of Portfolio</td></tr><tr><td>Borrow at the risk - free rate</td><td>-\$32.279</td></tr><tr><td>Buy 0.3178 Shares</td><td>+\$35.348</td></tr><tr><td>Total Value</td><td>= \$3.06</td></tr></table>

## Time 2

■ Again, if tick was down, the portfolio is now worth $0, do nothing the rest of the option's life and the portfolio matches the option payoffs since it expires worthless. 

■ If the tick was up, the portfolio is now worth $6.135. Adjust the portfolio in the following way: 

<table><tr><td>Position</td><td>Value of Portfolio</td></tr><tr><td>Borrow at the risk - free rate</td><td>-\$64.5754</td></tr><tr><td>Buy 0.583 Shares</td><td>+\$70.7116</td></tr><tr><td>Total Value</td><td>= \$6.135</td></tr></table>

## Time 3

■ Again, if tick was down, the portfolio is now worthless, matching the option's payoffs. 

- If the tick was up, the portfolio is now worth $12.26 and the option's payoffs are replicated by this portfolio. 

(b) Since the self-financing portfolio in part (a) matches the options payoffs, the option's value at time 0 must equal the time 0 value of the portfolio. Specifically, $C_t = 102 \times 0.173 - 16.1133 = \$1.53$ . 

(c) To hedge the position, simply follow the dynamic hedging portfolio outlined in part (a) with everything multiplied by 100. For example, at time 0, borrow $100 \times 16.1133 = \$1,611.33$ and buy $100 \times .173 = 17.3$ shares of the stock. Continue this scaling along the remainder of the tree. 

(d) If the market price of this call were $5, sell the call and use $1.53 of the proceeds to form the replicating portfolio. The remaining $3.47 is risk - free profit. 

6. (a) If $\mu = r$ , the expected value of $S_{t + \Delta}$ conditional on $S_{t}$ is 

$$
E ^ {p} [ S _ {t + \Delta} | S _ {t} ] = S _ {t} (1 + r)
$$

for the appropriate $p$ . With the process 

$$
S _ {t + \Delta} = S _ {t} + r S _ {t} + \sigma S _ {t} \epsilon_ {t}
$$

p must satisfy 

$$
S _ {t} (1 + r + \sigma) p + S _ {t} (1 + r - \sigma) (1 - p) = (1 + r) S _ {t}
$$

which is true for $p = \frac{1}{2}$ . This is the only choice for p which makes the discounted stock a martingale. 

(b) No, $p = \frac{1}{3}$ is not consistent since this measure does not make the discounted stock a martingale. 

(c) With risk premiums in the economy, the stock price process is not under the risk - neutral measure. Hence $p$ represents the empirical, statistical, or true measure for the stock. 

(d) It is only possible to determine the value of p statistically. This would involve calibrating a particular SDE to observed stock prices. A probability could then be inferred using a procedure similar to chapter 17, problem 1, part (d). 

7. (a) We want to choose $\Delta$ such that $5\Delta = \frac{200}{365}$ . Thus, $\Delta = \frac{40}{365}$ or 40 days. 

(b) $u = \exp \left\{ (0.12) \sqrt{\frac{40}{365}} \right\} = 1.0405.$ Thus, $d = \frac{1}{u} = 0.9611$ 

(c) The implied up probability is $p = \frac{(1 + r\Delta - d)}{(u - d)} = 0.5727$ . This is a risk neutral probability. 

(d) Stock price tree with $S_{0} = 100$ . 

$$
t = 0 \qquad t = 1 \qquad t = 2 \qquad t = 3 \qquad t = 4 \qquad t = 5
$$

$$
\begin{array}{c c c c c c} & & & & & 1 2 1. 9 7 2 5 \\ & & & & 1 1 7. 2 2 2 1 \\ & & & 1 1 2. 6 5 6 7 & & 1 1 2. 6 5 6 7 \\ & & 1 0 8. 2 6 9 2 & & 1 0 8. 2 6 9 2 \\ & 1 0 4. 0 5 2 5 & & 1 0 4. 0 5 2 5 & & 1 0 4. 0 5 2 5 \\ 1 0 0 & & 1 0 0 & & 1 0 0 \\ & 9 6. 1 0 5 4 & & 9 6. 1 0 5 4 & & 9 6. 1 0 5 4 \\ & & & 9 2. 3 6 2 4 & & 9 2. 3 6 2 4 \\ & & & & \text {88.7652} & \text {88.7652} \\ & & & & \text {85.3081} & \text {81.9857} \end{array}
$$

(e) The call premium tree is below. Work backwards from the terminal node at t = 5 where the call premium is simply; max (S $_{5}$ - 100, 0). For example, at t = 4, the top node is priced as $\frac{p \times 21.9725 + (1 - p) \times 12.6567}{1 + r\Delta} = \$17.8743$ . 

$$
t = 0 \qquad t = 1 \qquad t = 2 \qquad t = 3 \qquad t = 4 \qquad t = 5
$$

$$
\begin{array}{c c c c c c} & & & & & 2 1. 9 7 2 5 \\ & & & & 1 7. 8 7 4 3 & \\ & & & 1 3. 9 5 7 0 & & 1 2. 6 5 6 7 \\ & & 1 0. 5 1 1 3 & & 8. 9 2 1 5 & \\ 5. 4 7 0 3 & 7. 6 7 9 3 & & 6. 0 5 4 8 & & 4. 0 5 2 5 \\ & 2. 5 9 3 7 & & 1. 3 1 1 8 & & 0 \\ & & 0. 7 4 6 4 & & 0 & \\ & & & 0 & & 0 \\ & & & & 0 & \\ & & & & & 0 \end{array}
$$

Hence, the value of the call option at the present time, t = 0, is $5.47. 

## CHAPTER 3

1. Are the following sequences convergent? 

$$
\begin{array}{r l} & {\mathrm{(a)} \{X _ {n} \} _ {n = 1} ^ {\infty} = \{a, a ^ {2}, a ^ {3}, \ldots \}} \\ & {\qquad X _ {n} \left\{ \begin{array}{l l} \mathrm{convergesto0} & \mathrm{if} | a | <   1 \\ \mathrm{convergesto1} & \mathrm{if} a = 1 \\ \mathrm{diverges} & \mathrm{if} | a | > 1 \end{array} \right.} \\ & {\mathrm{(b)} \{X _ {n} \} _ {n = 1} ^ {\infty} = \left\{2, \frac {9}{4}, \frac {6 4}{2 7}, \ldots \right\} X _ {n} = \left(1 + \frac {1}{n}\right) ^ {n} \to e \approx 2. 7 1 8 2 8 \quad \mathrm{Convergentsince}} \end{array}
$$

$$
\begin{array}{r c l}\ln (X _ {n})&=&n \ln \left(\frac {n + 1}{n}\right)\\&=&\frac {\ln \left(\frac {n + 1}{n}\right)}{\frac {1}{n}}\\&&\mathrm {u s e L^ {\prime} hopital^ {\prime} s rule , numerator and denominator both approach zero as n\to\infty}\\&=&\frac {1}{\frac {n + 1}{n}} \left[ \frac {1}{n} - \frac {n + 1}{n ^ {2}} \right] (- n ^ {2})\\&=&\frac {n}{n + 1} \left[ - n + n + 1 \right]\\&=&\frac {n}{n + 1} \rightarrow 1\\\Rightarrow X _ {n}&\rightarrow&e ^ {1}\end{array}
$$

because ln is a continuous function which allows the interchange of the limit. 

$$
\mathrm{(c)} \{X _ {n} \} _ {n = 1} ^ {\infty} = \left\{0, - \frac {1}{2}, \frac {1}{6}, - \frac {1}{2 4}, \ldots \right\} X _ {n} = \frac {(- 1) ^ {n - 1}}{n !} \to 0 \quad \mathrm{Convergentsince}
$$

$$
| X _ {n} | = \frac {1}{n !} \rightarrow 0
$$

The yearly interest rate is 5% and the intervals, $\Delta$ , are chosen such that $n\Delta = 1$ . 

i. What is the gross return on $1 invested during Δ ? 

$$
\begin{array}{r c l} {1. 0 5} & = & {\left(1 + \frac {x}{n}\right) ^ {n}} \\ {\Rightarrow 1 + \frac {x}{n}} & = & {(1. 0 5) ^ {\frac {1}{n}}} \\ {\Rightarrow x} & = & {n \left[ 1. 0 5 ^ {\frac {1}{n}} - 1 \right] \quad \mathrm{andwith} n = \frac {1}{\Delta}} \\ & = & {\frac {1 . 0 5 ^ {\Delta} - 1}{\Delta}} \end{array}
$$

ii. What is the compound return during one year? Use results from problem 1, part (b). 

$$
\begin{array}{r l r}{1. 0 5}&=&{\left(1 + \frac {x}{n}\right) ^ {n}}\\&\rightarrow&{e ^ {x}}\end{array}
$$

In the limit, $e^x = 1.05$ which implies that $x = \ln (1.05) \approx .04879$ . 

2. If it exists, find the limit of the following sequences for $n = 1,2,3,\ldots$ 

(a) No limit 

$X_{n} = \left\{ \begin{array}{ll}1 & \mathrm{even~natural~numbers}\\ -1 & \mathrm{odd~natural~numbers} \end{array} \right.$ 

(b) No limit, function is periodic 

$$
X _ {n} = \left\{ \begin{array}{c l} 0 & n = 3, 6, 9, \ldots \\ - \frac {\sqrt {3}}{2} & n = 4, 5, 1 0, 1 1, \ldots \\ \frac {\sqrt {3}}{2} & n = 1, 2, 7, 8, \ldots \end{array} \right.
$$

(c) No limit, sequence oscillates worse than part (a) 

(d) No limit, the second term, $\frac{(-1)^n}{n}$ converges to 0 but the first term is part (b) which does not converge. 

Is $X_{n} = \sin \left(\frac{n\pi}{3}\right) + \frac{(-1)^{n}}{n}$ bounded? Yes, both components are bounded in absolute value by 1. 

3. Determine the following limits. 

(a) $\lim_{n\to\infty}\frac{(3+\sqrt{n})}{\sqrt{n}}=\lim_{n\to\infty}\frac{3}{\sqrt{n}}+1=1$ 

(b) $\lim_{n\to\infty}n^{\frac{1}{n}}=1$ 

$$
\begin{array}{r c l}\lim _ {n \to \infty} \ln \left(n ^ {\frac {1}{n}}\right)&=&\lim _ {n \to \infty} \frac {\ln (n)}{n}\\&=&\lim _ {n \to \infty} \frac {1}{n} \mathrm {by L^ {\prime} hopital^ {\prime} s rule}\\&\rightarrow&0\\\Rightarrow n ^ {\frac {1}{n}}&\rightarrow&e ^ {0} = 1\end{array}
$$

4. The sum $\sum_{k=1}^{n} \frac{1}{k!}$ equals $\sum_{k=0}^{n} \frac{1}{k!} - 1$ since $\frac{1}{0!} = 1$ . By definition, $\sum_{k=0}^{\infty} \frac{x^k}{k!} = e^x$ . The sum, $\sum_{k=0}^{n} \frac{1}{k!}$ , starting at $k = 0$ is the partial sum of $e^1$ . In the limit, $\sum_{k=1}^{n} \frac{1}{k!} \to e^1 - 1$ . Hence, $\sum_{k=1}^{n} \frac{1}{k!}$ converges to $e^1 - 1 \approx 1.718282$ . 

5. Show the partial sum $S_{n + 1} = \sqrt{3S_n}$ with $S_{1} = 1$ converges to 3. Claim: $S_{n} = 3^{\frac{2^{n - 1} - 1}{2^{n - 1}}}$ . 

(a) Base Case, n = 2 $S_{2} = \sqrt{3 \cdot 1} = 3^{\frac{1}{2}} = 3^{\frac{2^{1} - 1}{2^{1}}}$ 

(b) Assumption Assume formula true for $n = k$ 

$$
S _ {k} = 3 ^ {\frac {2 ^ {k - 1} - 1}{2 ^ {k - 1}}}
$$

(c) Induction Then, for $k + 1$ , want $S_{k+1} = 3^{\frac{2^{k} - 1}{2^{k}}}$ as the result. 

$$
\begin{array}{r c l} S _ {k + 1} & = & \sqrt {3 \cdot S _ {k}} \\ & = & \sqrt {3 \cdot 3 ^ {\frac {s ^ {k - 1} - 1}{s ^ {k - 1}}}} \\ & = & \sqrt {3 ^ {\frac {2 ^ {k - 1} + 2 ^ {k - 1} - 1}{2 ^ {k - 1}}}} \\ & = & 3 ^ {\frac {2 ^ {k} - 1}{2 ^ {k}}} \end{array}
$$

Thus, $\lim_{n\to \infty}S_n = 3^{\lim_{n\to \infty}\frac{2^n - 1}{2^n}} = 3.$ 

6. The series $\sum_{n=1}^{N}\frac{1}{n}$ is a harmonic series and does not converge. Despite the fact that $\frac{1}{n}$ decreases to zero, the decrease is not rapid enough to ensure the infinite sum converges. 

$$
\sum_ {n = 1} ^ {N} \frac {1}{n} = 1 + \left(\frac {1}{2}\right) + \left(\frac {3}{4} + \frac {1}{4}\right) + \left(\frac {1}{5} + \frac {1}{6} + \frac {1}{7} + \frac {1}{8}\right) + \left(\frac {1}{9} + \dots + \frac {1}{1 6}\right) + \dots
$$

The terms in brackets, ( ), all add up to greater than or equal to $\frac{1}{2}$ with $2^{k}$ elements in each bracket (i.e. 1, 2, 4, 8, ... terms). Therefore, $\sum_{n=1}^{N}\frac{1}{n}>1+\frac{1}{2}+\frac{1}{2}+\frac{1}{2}+\ldots$ and the series diverges. 

7. The series, $X_{n} = aX_{n - 1} + 1$ , will converge provided that $|a| < 1$ . This is an autoregressive AR(1) process. It can be written as a partial sum through successive backward substitution. 

$$
\begin{array}{r c l} X _ {n} & = & a X _ {n - 1} + 1 \quad \text {substituting in the previous value} X _ {n - 1} = a X _ {n - 2} + 1 \\ & = & a ^ {2} X _ {n - 2} + a + 1 \quad \text {after further substitution} \\ & = & a ^ {3} X _ {n - 3} + a ^ {2} + a + 1 \\ & & \vdots \\ & = & a ^ {n} X _ {0} + \sum_ {k = 0} ^ {n - 1} a ^ {k} \end{array}
$$

8. The function $f(x) = x^{3}$ is a monotonically increasing function for $x \in [0,1]$ . Therefore, the left “endpoint” underestimates the value of the integral while the right “endpoint” overestimates the integral. 

$$
\mathrm{(a)} \int_ {0} ^ {1} x ^ {3} d x = \left. \frac {1}{4} x ^ {4} \right| _ {0} ^ {1} = \frac {1}{4}
$$

(b) Choose an evenly spaced partition for simplicity such as $x_{0}=0$ , $x_{1}=\frac{1}{4}$ , $x_{2}=\frac{1}{2}$ , $x_{3}=\frac{3}{4}$ , and $x_{4}=1$ . The terms $x_{i}-x_{i-1}\forall i=1,\ldots,4$ always evaluate to $\frac{1}{4}$ . Therefore, with $f(x_{i})=x_{i}^{3}$ , the sum becomes 

$$
\begin{array}{r c l} \sum_ {i = 1} ^ {4} f (x _ {i}) (x _ {i} - x _ {i - 1}) & = & \frac {1}{4} \left[ \frac {1 + 8 + 2 7 + 6 4}{6 4} \right] \\ & = & \frac {3}{8} \quad \left(= \frac {2 4}{6 4}\right) \end{array}
$$

$$
\begin{array}{r c l} \sum_ {i = 1} ^ {4} f (x _ {i - 1}) (x _ {i} - x _ {i - 1}) & = & \frac {1}{4} \left[ \frac {0 + 1 + 8 + 2 7}{6 4} \right] \\ & = & \frac {9}{6 4} \end{array}
$$

(c) As expected, the true value $\frac{1}{4} = \frac{16}{64}$ lies between the two “endpoints”, $\frac{9}{64} < \frac{16}{64} < \frac{24}{64}$ . 

9. (a) The integral has no closed form solution. It can be simplified using successive applications of integration by parts. As this is tedious, computer software such as MATLAB can be utilized with the following commands. 

x=sym('x') 

int(x*sin(pi/x),0,1) 

The result generated by MATLAB is 

$$
\int_ {0} ^ {1} f (x) d x = \frac {\pi^ {2}}{2} \int_ {0} ^ {\pi} \frac {s i n (t)}{t} d t - \frac {\pi}{2} - \frac {\pi^ {3}}{4}
$$

The integral $\int_{0}^{\pi}\frac{sin(t)}{t}dt$ can be evaluated numerically with the following MATLAB command. quad8('integral', 0, pi) 

where the argument integral is a separate m - file program 

function y=integral(x) 

y = (sin(x)) / x; 

MATLAB generated 1.8511091 as the approximation to $\int_0^\pi \frac{sin(t)}{t} dt$ . Thus, the entire expression is approximately $\frac{\pi^2}{2} (1.8511091) - \frac{\pi}{2} -\frac{\pi^3}{4}\approx -0.187508$ . 

(b) Approximation of $\int_0^1 f(x)dx$ . Choose the same evenly spaced partition of with $\frac{1}{4}$ for the mesh size. Since the intensity of the fluctuations increases as $x$ approaches zero, placing a finer grid near zero could improve performance. Usually, for a given number of nodes, placing more nodes in regions where the function fluctuates more intensely increases the accuracy of the approximation. Let $x_0 = 0$ , $x_1 = \frac{1}{4}$ , $x_2 = \frac{1}{2}$ , $x_3 = \frac{3}{4}$ , and $x_4 = 1$ . The terms $x_i - x_{i-1} \forall i = 1, \ldots, 4$ evaluate to $\frac{1}{4}$ . Therefore, with $f(x_i) = x_i\left(\sin\left(\frac{\pi}{x_i}\right)\right)$ , the sum becomes 

$$
\begin{array}{r c l} \sum_ {i = 1} ^ {4} f (x _ {i}) (x _ {i} - x _ {i - 1}) & = & \frac {1}{4} \left[ 0 + 0 - \frac {3 \sqrt {3}}{8} + 0 \right] \\ & = & - \frac {3 \sqrt {3}}{4 8} \approx -. 1 0 8 2 5 \end{array}
$$

$$
\begin{array}{r l r} \sum_ {i = 1} ^ {4} f (x _ {i - 1}) (x _ {i} - x _ {i - 1}) & = & \frac {1}{4} \left[ 0 + 0 + 0 - \frac {3 \sqrt {3}}{8} \right] \\ & = & - \frac {3 \sqrt {3}}{4 8} \approx -. 1 0 8 2 5 \end{array}
$$

(c) The sums are not accurate. 

(d) The sums do not approximate the integral very well since the function oscillates rapidly. 

10. Calculate the partial derivatives with respect to $x, y$ , and $z$ of the function $f(x,z,y) = \frac{x + y + z}{(1 + x)(1 + y)(1 + z)}$ . 

$$
\begin{array}{r c l} \frac {\partial \left(\frac {(x + y + z) (1 + x) ^ {- 1}}{(1 + y) (1 + z)}\right)}{\partial x} & = & \frac {1}{(1 + x) (1 + y) (1 + z)} - \frac {(x + y + z)}{(1 + x) ^ {2} (1 + y) (1 + z)} \\ & = & \frac {1}{(1 + x) (1 + y) (1 + z)} \left[ 1 - \frac {x + y + z}{1 + x} \right] \\ & = & \frac {1}{(1 + x) (1 + y) (1 + z)} \left[ \frac {1 + x - x - y - z}{1 + x} \right] \\ & = & \frac {1 - y - z}{(1 + x) ^ {2} (1 + y) (1 + z)} \end{array}
$$

The partial derivatives for y and z follow immediately from the above calculations. 

$$
{f _ {y}} = {\frac {1 - x - z}{(1 + x) (1 + y) ^ {2} (1 + z)}}
$$

$$
{f _ {z}} = {\frac {1 - x - y}{(1 + x) (1 + y) (1 + z) ^ {2}}}
$$

## CHAPTER 4

1. (a) The expected gain for a bet on the incumbent winning is 0.6 × $1,000 - 0.4 × $1,500 = $0. 

(b) Yes, the value of $p$ is important as it determines the expected gain. 

(c) Two people taking this bet would not necessarily agree on p. Neither person would necessarily be correct since p is not observed. The assessment of p is subjective. 

(d) Yes, statistics can be employed to determine p. One could use survey sampling as in political polls to determine the true p or one could look at past data and try to estimate p historically. 

(e) The statistician's assessment of $p$ is crucial. The assessment provides an objective, although not perfectly accurate, assessment of $p$ . 

(f) How much one is willing to pay for this bet depends on an individual's level of risk aversion since $p$ is not the risk - neutral probability. 

2. (a) One could go long $R^{*}$ and short $R$ . The risk - free payoff is $500 regardless of the election's outcome. 

(b) No, the value of $p$ is not important in selecting this portfolio. The payoff of the portfolio is independent of the election outcome. Not unless one knows the portfolio and it's payoffs can the portfolio help determine the unknown $p$ . 

(c) A statistician or econometrician would play no role in making these decisions since the outcome of the election does not effect the portfolio payoffs. The payoffs are independent of p. 

## CHAPTER 5

1. Two discrete random variables X, Y that assume either the value 0 or 1. 

(a) Marginal Distributions. 

$$
P (X = 1) = P (X = 1 | Y = 1) P (Y = 1) + P (X = 1 | Y = 0) P (Y = 0) = . 6 0
$$

$$
P (X = 0) = P (X = 0 | Y = 1) P (Y = 1) + P (X = 0 | Y = 0) P (Y = 0) = . 4 0
$$

$$
P (Y = 1) = P (Y = 1 | X = 1) P (X = 1) + P (Y = 1 | X = 0) P (X = 0) = . 3 5
$$

$$
P (Y = 0) = P (Y = 0 | X = 1) P (X = 1) + P (Y = 0 | X = 0) P (X = 0) = . 6 5
$$

(b) Independence. $X \perp Y \Rightarrow E[XY] = E[X]E[Y]$ . 

The expectation of XY, $E[XY]$ , is .20 since X and Y must both be nonzero for the expectation to be nonzero. Therefore, the only element in the matrix of concern is the entry where X = Y = 1. The expectation of X is simply the probability that X is 1 and similarly for Y. 

$$
\begin{array}{r c l} E [ X ] E [ Y ] & = & \left[ (1) P (X = 1) + (0) P (X = 0) \right] \left[ (1) P (Y = 1) + (0) P (Y = 0) \right] \\ & = & P (X = 1) P (Y = 1) \\ & = & (. 6 0) (. 3 5) \\ & = & . 2 1 \\ & \neq & . 2 0 \quad \mathrm{NotIndependent} \end{array}
$$

(c) from above, $E[X] = .60$ and $E[Y] = .35$ 

(d) Conditional Distribution. 

$$
P (X = 1 | Y = 1) = \frac {P (X = 1 , Y = 1)}{P (Y = 1)} = \frac {. 2}{. 3 5}
$$

$$
P (X = 0 | Y = 1) = \frac {P (X = 0 , Y = 1)}{P (Y = 0)} = \frac {. 1 5}{. 3 5}
$$

(e) Conditional Expectation $E[X|Y = 1]$ and Conditional Variance $Var[X|Y = 1]$ . 

$$
\begin{array}{r c l} E [ X | Y = 1 ] & = & (1) P (X = 1 | Y = 1) + (0) P (X = 0 | Y = 1) \\ & = & P (X = 1 | Y = 1) \\ & = & \frac {P (X = 1 , Y = 1)}{P (Y = 1)} \\ & = & \frac {. 2}{. 3 5} \end{array}
$$

$$
\begin{array}{r c l} V a r [ X | Y = 1 ] & = & E \left[ X - E [ X ] | Y = 1 \right] ^ {2} \\ & = & \left(1 - \frac {. 2}{. 3 5}\right) ^ {2} P (X = 1 | Y = 1) + \left(\frac {- . 2}{. 3 5}\right) ^ {2} P (X = 0 | Y = 1) \\ & = & \left(1 - \frac {. 2}{. 3 5}\right) ^ {2} \frac {. 2}{. 3 5} + \left(\frac {. 2}{. 3 5}\right) ^ {2} \frac {. 1 5}{. 3 5} \\ & = & . 2 4 4 8 9 \end{array}
$$

2. (a) The random variable is binomial, $X_{n} = \sum_{i=1}^{n} B_{i}$ , where $B_{i}$ are independent Bernoulli random variables with distribution 

$B_{i} = \left\{ \begin{array}{ll}1 & \mathrm{~w i t h ~ p r o b a b i l i t y ~ } \\ 0 & \mathrm{~w i t h ~ p r o b a b i l i t y ~ } 1 - p \end{array} \right.$ 

Calculate $P(X_4 > K)$ for $k = 0,1,2,3,4$ with $\binom{n}{m} = \frac{n!}{m!(n - m)!}$ . 

$$
\begin{array}{r c l} P (X _ {4} > 0) & = & 1 - P (X _ {4} = 0) = 1 - \left( \begin{array}{l} 4 \\ 0 \end{array} \right) p ^ {0} (1 - p) ^ {4} = 1 - (1 - p) ^ {4} \\ P (X _ {4} > 1) & = & 1 - P (X _ {4} = 0) - P (X _ {4} = 1) \\ & = & 1 - (1 - p) ^ {4} - \left( \begin{array}{l} 4 \\ 1 \end{array} \right) p ^ {1} (1 - p) ^ {3} \\ & = & 1 - (1 - p) ^ {4} - 4 p ^ {1} (1 - p) ^ {3} \\ & \vdots & \\ P (X _ {4} > 4) & = & 0 \end{array}
$$

The general formula for $0 \leq k \leq 4$ is 

$$
P (X _ {4} > k) = 1 - \sum_ {i = 0} ^ {k} \left( \begin{array}{l} 4 \\ i \end{array} \right) p ^ {i} (1 - p) ^ {k - i}
$$

Plot the distribution function. Assume $p = \frac{1}{2}$ . 

%Calculate Binomial Density and Cumulative Density 

$$
\begin{array}{l} \text {\%Method 1} \\ \text {pr = .5;} \\ \text {n = 4;} \\ \text {for i = 1:5} \\ \quad \mathrm {p(i) = (factorial(n) / (factorial(i - 1)*factorial(n - i + 1)))*pr^ {(i - 1)*(1- pr) ^ {(n - i + 1)}} ;} \\ \text {and} \end{array}
$$

```matlab
for i=1:5
    MATLABp(i) = binopdf(i-1,n,pr);
end

%Binomial Cumulative Density Function - Two Methods
%Method 1
cump(1) = p(1);
for i=2:5
    cump(i) = p(i) + cump(i-1);
end

%Method 2 (built in MATLAB function)
for i=1:5
    cumMATLABp(i) = binocdf(i-1,n,pr);
end 
```

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5882bd1f-b733-4ed9-8bdc-4c98ae290af0/c9a763c0b2b652ca0b2aba2e26b753f2bd70204c3c3f11e618c7825f2bbf12c8.jpg)



FIGURE 0.8 Binomial Density with p = .5 and n = 4


(b) $E[X_{3}] = 3p$ . The expectation of a binomial with probability p is np. 

3. Exponential distribution with parameter $\lambda$ has cumulative distribution function $P(Z < z) = 1 - e^{-\lambda z}$ . 

(a) Density function $f(z) = \frac{\partial P(Z < z)}{\partial z} = \lambda e^{-\lambda z}$ 

$$
\mathrm{(b)} E [ Z ] = \int_ {0} ^ {\infty} z f (z) d z
$$

$$
\begin{array}{r c l} E [ Z ] & = & \lambda \int_ {0} ^ {\infty} z e ^ {- \lambda z} d z \qquad \mathrm{useIntegrationbyparts} \\ & = & - z e ^ {- \lambda z} \big | _ {0} ^ {\infty} + \int_ {0} ^ {\infty} e ^ {- \lambda z} d z \\ & = & \frac {1}{\lambda} \end{array}
$$

$$
\mathrm{(c)} V a r [ Z ] = E [ Z ^ {2} ] - E [ Z ] ^ {2}
$$

$$
\begin{array}{r c l} E [ Z ^ {2} ] & = & \lambda \int_ {0} ^ {\infty} z ^ {2} e ^ {- \lambda z} d z \qquad \mathrm{useIntegrationbypartstwice} \\ & = & \frac {2}{\lambda^ {2}} \\ \Rightarrow V a r [ Z ] & = & \frac {2}{\lambda^ {2}} - \frac {1}{\lambda^ {2}} \\ & = & \frac {1}{\lambda^ {2}} \end{array}
$$

(d) $Z_{1}$ and $Z_{2}$ are independent and distributed $Z_{1} \sim exp(\lambda)$ , $Z_{2} \sim exp(\lambda)$ . Their sum is distributed according to the two parameter gamma density. In general, for $n$ independent random variables, their sum has a moment generating function equal to the product of the individual moment generating functions. A convolution could also be employed. The product of exponential moment generating functions, $I(t) = \frac{\lambda}{\lambda - t}$ , is 

$$
\begin{array}{r c l} I ^ {2} (t) & = & \left(\frac {\lambda}{\lambda - t}\right) \left(\frac {\lambda}{\lambda - t}\right) \\ & = & \left(\frac {\lambda}{\lambda - t}\right) ^ {2} \end{array}
$$

This is the unique moment generating function for a $\Gamma(2, \lambda)$ density. The convolution approach yields 

$$
\begin{array}{r c l} {f _ {S} (s)} & = & {\int_ {0} ^ {s} \lambda e ^ {- \lambda x} \lambda e ^ {- \lambda (s - x)} d x} \\ & = & {\lambda^ {2} e ^ {- \lambda s} \int_ {0} ^ {s} d x} \\ & = & {\lambda^ {2} s e ^ {- \lambda s}} \end{array}
$$

which is a $\Gamma(2, \lambda)$ density. 

(e) The mean and variance of a $\Gamma(2, \lambda)$ are $\frac{2}{\lambda}$ and $\frac{2}{\lambda^2}$ respectively. These can be obtained from the moment generating function or through direct integration. For example, the mean is 

$$
\begin{array}{r c l} \int_ {0} ^ {\infty} s f _ {S} (s) d s & = & \lambda^ {2} \int_ {0} ^ {\infty} s ^ {2} e ^ {- \lambda s} d s \\ & = & 2 \lambda \int_ {0} ^ {\infty} s e ^ {- \lambda s} d s \\ & = & \frac {2}{\lambda} \end{array}
$$

use Integration by parts 

another Integration by parts 

The computation of the second moment proceeds in a similar fashion and equals 

$$
\int_ {0} ^ {\infty} s ^ {2} f _ {S} (s) d s = \lambda^ {2} \int_ {0} ^ {\infty} s ^ {3} e ^ {- \lambda s} d s = \frac {6}{\lambda^ {2}}
$$

Therefore, the variance equals $\frac{6}{\lambda^2} - \frac{4}{\lambda^2} = \frac{2}{\lambda^2}$ . 

4. $Z \sim \text{Poisson}(\lambda)$ if $\text{Prob}(Z = k) = \frac{\lambda^{k} e^{-\lambda}}{k!}$ where k is a nonnegative integer. 

(a) Show $\sum_{k=0}^{\infty} Prob(Z = k) = 1$ . 

$$
\begin{array}{r c l} \sum_ {k = 0} ^ {\infty} P r o b (Z = k) & = & \sum_ {k = 0} ^ {\infty} \frac {\lambda^ {k} e ^ {- \lambda}}{k !} \\ & = & e ^ {- \lambda} \sum_ {k = 0} ^ {\infty} \frac {\lambda^ {k}}{k !} \\ & = & e ^ {- \lambda} e ^ {\lambda} \\ & = & 1 \end{array}
$$

(b) Calculate the mean and variance of $Z$ . Moment generating function produce the required solutions directly. 

$$
\begin{array}{r c l} E [ Z ] & = & \sum_ {k = 0} ^ {\infty} k \frac {\lambda^ {k} e ^ {- \lambda}}{k !} \\ & = & \sum_ {k = 1} ^ {\infty} k \frac {\lambda^ {k} e ^ {- \lambda}}{k !} \\ & = & \sum_ {k = 1} ^ {\infty} \frac {\lambda^ {k} e ^ {- \lambda}}{(k - 1) !} \quad \mathrm{changeofvariables,} m = k - 1 \\ & = & e ^ {- \lambda} \sum_ {m = 0} ^ {\infty} \frac {\lambda^ {m + 1}}{m !} \\ & = & \lambda e ^ {- \lambda} \sum_ {m = 0} ^ {\infty} \frac {\lambda^ {m}}{m !} \\ & = & \lambda \end{array}
$$

$$
\begin{array}{r c l} E [ Z ^ {2} ] & = & e ^ {- \lambda} \sum_ {k = 0} ^ {\infty} k ^ {2} \frac {\lambda^ {k}}{k !} \\ & = & \sum_ {k = 1} ^ {\infty} k ^ {2} \frac {\lambda^ {k} e ^ {- \lambda}}{k !} \\ & = & \sum_ {k = 1} ^ {\infty} k \frac {\lambda^ {k} e ^ {- \lambda}}{(k - 1) !} \quad \text {change of variables, m = k - 1} \\ & = & e ^ {- \lambda} \sum_ {m = 0} ^ {\infty} (m + 1) \frac {\lambda^ {m + 1}}{m !} \\ & = & e ^ {- \lambda} \sum_ {m = 0} ^ {\infty} m \frac {\lambda^ {m + 1}}{m !} + e ^ {- \lambda} \sum_ {m = 0} ^ {\infty} \frac {\lambda^ {m + 1}}{m !} \\ & = & \lambda e ^ {- \lambda} \sum_ {m = 0} ^ {\infty} m \frac {\lambda^ {m}}{m !} + e ^ {- \lambda} \sum_ {m = 0} ^ {\infty} \frac {\lambda^ {m + 1}}{m !} \\ & = & (\lambda + 1) e ^ {- \lambda} \sum_ {m = 0} ^ {\infty} \frac {\lambda^ {m + 1}}{m !} \\ & = & (\lambda + 1) \lambda \end{array}
$$

$$
\begin{array}{r c l} {V a r [ Z ]} & = & {E [ Z ^ {2} ] - E [ Z ] ^ {2}} \\ & = & {\lambda^ {2} + \lambda - \lambda^ {2}} \\ & = & {\lambda} \end{array}
$$

## CHAPTER6

1. (a) If $M_{t} = E(Y|I_{t})$ then by the law of iterated expectations 

$$
\begin{array}{r c l} E (M _ {t + s} | I _ {t}) & = & E [ E (Y | I _ {t + s}) | I _ {t} ] \\ & = & E (Y | I _ {t}) \\ & = & M _ {t}, \end{array}
$$

and $M_{t}$ is a martingale. 

(b) Yes, every conditional expectation is a martingale provided the conditioning is with respect to the same filtration. 

2. (a) $E(X_4|I_1) = X_1$ , $E(X_4|I_2) = X_2$ , and $E(X_4|I_4) = X_4$ . 

(b) If $Z_{i} = E(X_{4}|I_{i})$ , then $Z_{i}$ is a martingale by problem 1 above. 

(c) Define $V_{i} = B_{i} + \sqrt{i}$ . For k > 0 consider 

$$
\begin{array}{r c l} E (V _ {i + k} | V _ {i}) & = & E (B _ {i + k} + \sqrt {i + k} | B _ {i} + \sqrt {i}) \\ & = & E (B _ {i + k} | B _ {i} + \sqrt {i}) + \sqrt {i + k} \\ & = & B _ {i} + \sqrt {i + k} \end{array}
$$

which is not equal to $B_{i} + \sqrt{i}$ . 

The random process $V_{i}$ is a submartingale since $\sqrt{i} > 0$ and $B_{i}$ is iid with $E(B_{i}) = 0$ . Therefore, with $i \geq j$ , $E[V_{i}|I_{j}] \geq V_{j}$ . 

(d) Yes, transform $V_{i}$ by subtracting the deterministic component $\sqrt{i}$ . Then, $V_{i} = B_{i}$ and $V_{i}$ is now a martingale. 

(e) No, $B_{i}$ are iid random variables. For $V_{i}$ to be a martingale, it must be the case that $E(B_{i}) = -\sqrt{i}$ for all $i$ . This is not possible. 

3. (a) If $X_{t} = 2W_{t} + t$ then 

$$
\begin{array}{r c l} E (X _ {t + s} | \mathcal {I} _ {t}) & = & E (2 W _ {t + s} + (t + s) | \mathcal {I} _ {t}) \\ & = & 2 W _ {t} + (t + s) \\ & \neq & 2 W _ {t} + t. \end{array}
$$

$X_{t}$ is not a martingale. 

(b) If $X_{t} = W_{t}^{2}$ then 

$$
\begin{array}{r c l} E [ X _ {t + s} | \mathcal {I} _ {t} ] & = & E [ W _ {t + s} ^ {2} | \mathcal {I} _ {t} ] \\ & = & W _ {t} ^ {2} + s \\ & \neq & W _ {t} ^ {2}, \end{array}
$$

$X_{t}$ is not a martingale. However, $W_{t}^{2} - t$ is a martingale. The second equality follows from 

$$
\begin{array}{r c l} W _ {t + s} ^ {2} & = & (W _ {t + s} - W _ {t}) ^ {2} + 2 W _ {t + s} W _ {t} - W _ {t} ^ {2} \\ E _ {t} [ W _ {t + s} ^ {2} ] & = & E _ {t} [ (W _ {t + s} - W _ {t}) ^ {2} + 2 W _ {t + s} W _ {t} - W _ {t} ^ {2} ] \\ & = & V a r (W _ {t + s} - W _ {t}) + 2 W _ {t} E _ {t} [ W _ {t + s} ] - W _ {t} ^ {2} \\ & = & s + 2 W _ {t} ^ {2} - W _ {t} ^ {2} \\ & = & s + W _ {t} ^ {2} \end{array}
$$

(c) If $X_{t} = W_{t}t^{2} - 2\int_{0}^{t}sW_{s}ds$ then 

$$
\begin{array}{r c l} E [ X _ {t + s} | \mathcal {I} _ {t} ] & = & E \left[ W _ {t + s} (t + s) ^ {2} - 2 \int_ {0} ^ {t + s} u W _ {u} d u \bigg | \mathcal {I} _ {t} \right] \\ & = & W _ {t} (t + s) ^ {2} - 2 \int_ {0} ^ {t} s W _ {s} d s - 2 E _ {t} \left[ \int_ {t} ^ {t + s} u W _ {u} d u \right] \\ & = & W _ {t} t ^ {2} - 2 \int_ {0} ^ {t} s W _ {s} d s + s (2 t + s) W _ {t} - 2 E _ {t} \left[ \int_ {t} ^ {t + s} u W _ {u} d u \right] \end{array}
$$

$X_{t}$ is a martingale as the last two terms cancel. The integral $\int_0^{t + s}uW_u du$ equals 

$$
\int_ {0} ^ {t + s} u W _ {u} d u = \int_ {0} ^ {t} s W _ {s} d s + \int_ {t} ^ {t + s} u W _ {u} d u
$$

and the result is a consequence of 

$$
\begin{array}{r c l} 2 E _ {t} \left[ \int_ {t} ^ {t + s} u W _ {u} d u \right] & = & 2 \int_ {t} ^ {t + s} u E _ {t} \left[ W _ {u} \right] d u \\ & = & 2 W _ {t} \int_ {t} ^ {t + s} u d u \\ & = & W _ {t} \left[ (t + s) ^ {2} - t ^ {2} \right] \\ & = & s (2 t + s) W _ {t} \end{array}
$$

which implies that $E[X_{t + s}|\mathcal{I}_t] = W_tt^2 - 2\int_0^t sW_sd = X_t$ . 

4. Given the representation 

$$
M _ {T} (X _ {t}) = M _ {0} (X _ {0}) + \int_ {0} ^ {t} g (t, X _ {t}) d W _ {t}
$$

with $dX_{t} = \mu dt + \sigma dW_{t}$ . The right hand side is always a martingale as $g(t, X_{t})$ is adapted to the filtration generated by $W_{t}$ . The Ito integral is a martingale and the initial term is constant and therefore a martingale. In all cases, the left hand side is also a martingale. Determine $g(\cdot, \cdot)$ for the following 

(a) $M_T(X_T) = W_T$ . Let $g(t,X_t) = 1$ . Since $W_0 = 0$ 

$$
\begin{array}{r c l} W _ {T} & = & \int_ {0} ^ {T} d W _ {t} \\ & = & W _ {0} + \int_ {0} ^ {T} g (t, W _ {t}) d W _ {t} \\ & = & M _ {0} (W _ {0}) + \int_ {0} ^ {T} g (t, X _ {t}) d W _ {t} \end{array}
$$

(b) $M_T(X_T) = W_T^2 - T$ . Employ the relationship $W_T^2 - T = 2 \int_0^T W_t dW_t$ (verify using Ito's lemma). Let $g(t, X_t) = 2W_t$ and the result follows. 

(c) $M_T(X_T) = e^{W_T - \frac{1}{2} T}$ . The function $g(t,X_t)$ is solved by using a trivial special case of Ito's integration by parts formula. 

$$
X _ {T} Y _ {T} = X _ {0} Y _ {0} + \int_ {0} ^ {T} X _ {t} d Y _ {t} + \int_ {0} ^ {T} Y _ {t} d X _ {t} + \left\langle X _ {t}, Y _ {t} \right\rangle_ {T}
$$

Define 

$$
X _ {t} = e ^ {W _ {t} - \frac {1}{2} t} \qquad X _ {0} = 1 \qquad d X _ {t} = X _ {t} d W _ {t}
$$

and 

$$
Y _ {t} = 1 \qquad Y _ {0} = 1 \qquad d Y _ {t} = 0
$$

The Ito integration by part formula reduces to 

$$
e ^ {W _ {T} - \frac {1}{2} T} = 1 + \int_ {0} ^ {T} e ^ {W _ {t} - \frac {1}{2} t} d W _ {t}
$$

Therefore, the function $g(t,X_t)$ equals $e^{W_t - \frac{1}{2} t}$ . 

These three exercises are applications of the martingale representation theorem. In financial theory, the function $g(t, X_{t})$ operates as a “hedge” parameter against the Brownian motion. It represents the sensitivity of the function $M_{t}(X_{t})$ to a movement in the Brownian motion. The function $M_{t}(X_{t})$ could generate a call option as the next example illustrates. 

5. In theory, the representation is possible. The difficulty is that $X_{t} = S_{t}$ may not be a martingale under the empirical measure involving $W_{t}$ . In general the call option has the form 

$$
M _ {T} (S _ {T}) = M _ {0} (S _ {0}) + \int_ {0} ^ {T} \phi (t) d S _ {t}
$$

where $S_{t}$ is under the risk - neutral measure. For example, $dS(t) = \sigma S_{t} d\tilde{W}_{t}$ in the Black Scholes model but the stock price process is now under the risk - neutral measure, not the empirical measure. The term $\phi(t)$ is the hedge parameter which equals $\frac{\partial C_K(t,S_t)}{\partial S_t}$ for the Black Scholes model; the partial derivative of the call with respect to the underlying stock. Continuing with the Black Scholes model to illustrate the difficulty, the call option can be expressed as 

$$
M _ {T} (S _ {T}) = M _ {0} (S _ {0}) + \int_ {0} ^ {T} \phi (t) \sigma S _ {t} d \tilde {W} _ {t}
$$

However, the representation does not occur under the empirical measure involving $W_{t}$ but with a transformed Brownian motion $\tilde{W}_{t}$ under the risk-neutral measure. A representation using $W_{t}$ would introduce a risk premium and a corresponding non constant additional term. This additional term would make the representation impossible. 

## CHAPTER7

1. Consider the geometric Brownian motion model, $S_{t} = S_{0} e^{\mu t + \sigma W_{t}}$ , used in Black Scholes. Here, the term $-\frac{1}{2} \sigma^{2} t$ has been omitted from the exponent which differs from chapter 11. Under the risk-neutral measure, the drift is set equal to r in either case. Only the risk premium differs between the two models but call values remain unchanged as the stock price process equals 

$$
\frac {d S _ {t}}{S _ {t}} = r d t + \sigma d W _ {t}
$$

under the risk - neutral measure. 

(a) Use the MATLAB command 

$\mathrm{x = normrnd(0,sqrt(.25),4,1)}$ 

to generate four normal random numbers with mean 0 and variance .25. Assume that $S_0 = 1$ for simplicity. One particular set of 4 draws (a MATLAB program is provided below for repeated drawings) produced the values .0873, -.0934, .3629, and -.2942. The path of the Brownian motion involves adding these values together over time 

$$
W _ {0} = 0, W _ {\frac {1}{4}} = . 0 8 7 3, W _ {\frac {1}{2}} = -. 0 0 6 1, W _ {\frac {3}{4}} = . 3 5 6 8, \mathrm{and} W _ {1} = . 0 6 2 6
$$

One possible stock price path is 

$$
\begin{array}{r c l} S _ {0} & = & 1 \\ S _ {\frac {1}{4}} & = & e x p \left\{(. 0 1) \frac {1}{4} + (. 1 5) W _ {\frac {1}{4}} \right\} \\ & = & e x p \left\{(. 0 1) \frac {1}{4} + (. 1 5) (. 0 8 7 3) \right\} \approx 1. 0 1 5 7 \\ S _ {\frac {1}{2}} & = & e x p \left\{(. 0 1) \frac {1}{2} + (. 1 5) W _ {\frac {1}{2}} \right\} \\ & = & e x p \left\{(. 0 1) \frac {1}{2} + (. 1 5) (-. 0 0 6 1) \right\} \approx 1. 0 0 4 1 \end{array}
$$

$\begin{array}{rcl}S_{\frac{3}{4}} & = & exp\left\{(.01)\frac{3}{4} +(.15)W_{\frac{3}{4}}\right\} \\ & = & exp\left\{(.01)\frac{3}{4} +(.15)(.3568)\right\} \approx 1.0629 \\ S_1 & = & exp\left\{(.01)\frac{1}{1} +(.15)W_1\right\} \\ & = & exp\left\{(.01)\frac{1}{1} +(.15)(.0626)\right\} \approx 1.0196 \end{array}$ 

Program and accompanying graphs (different draws than presented above) 

```matlab
mu = .01;
sigma = .15;
T = 1;
K = 1.5;
S0 = 1;
%n is the number of discretizations for T
%part (a), n=4
%part (b), n=8
n = 4;
delta = T/n;

%generate Brownian motions
bm=zeros(n,1);
%cbm is the cumulative Brownian motion
cbm=zeros(n,1);
cbm(1) = bm(1);

for j=2:n
    bm(j) = normrnd(0,sqrt(delta));
    cbm(j) = cbm(j-1) + bm(j);
end

axis=(0:delta:T);
newcbm=[0;cbm]';
%generate stock prices
stock = zeros(n,1);

for j=1:n
    stock(j) = S0 * exp((mu*j*delta) + sigma*cbm(j));
end

newstock=[S0;stock]';
%graph Brownian motion and stock
subplot(2,1,1), plot(axis,newcbm)
hold on
plot(axis,newcbm,'*')
xlabel('Time')
title('Brownian Motion Path')
hold off

subplot(2,1,2), plot(axis,newstock) 
```

```csv
hold on
plot(axis,newstock,'*')
xlabel('Time')
title('Stock Price Path')
hold off 
```

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5882bd1f-b733-4ed9-8bdc-4c98ae290af0/764d79727ee7582a31ad285009564d98afe604d2c09455aaa0be8a18d9e74e60.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5882bd1f-b733-4ed9-8bdc-4c98ae290af0/6d3618db58f05e3f8b5d7df490b31e990107cb73d93e5439c33bca39fefbad5b.jpg)



FIGURE 0.9 Brownian Motion and Stock Price Paths


(b) Repeat exercise for 8 subdivisions of interval with random variables approximating the Brownian motion having variance equal to $\frac{1}{8} = .125$ . 

x=normrnd(0,sqrt(.125),8,1) 

Using the above command generates eight random numbers .0841, -.3563, -.2624, .3826, -.0465, .1378, .0311, and -.2247. Use the same MATLAB program as above with n=8 instead of n=4 for repeated simulations. The path of the Brownian motion is 

$W_{0} = 0$ , $W_{\frac{1}{8}} = .0841$ , $W_{\frac{2}{8}} = -.2722$ , $W_{\frac{3}{8}} = -.5345$ , $W_{\frac{4}{8}} = -.1519$ , $W_{\frac{5}{8}} = -.1984$ , $W_{\frac{6}{8}} = -.0605$ , $W_{\frac{7}{8}} = -.0294$ , and $W_{1} = -.2541$ 

One possible stock price path is 

$$
\begin{array}{r c l} S _ {0} & = & 1 \\ S _ {\frac {1}{8}} & = & e x p \left\{(. 0 1) \frac {1}{8} + (. 1 5) W _ {\frac {1}{8}} \right\} \\ & = & e x p \left\{(. 0 1) \frac {1}{8} + (. 1 5) (. 0 8 4 1) \right\} \approx 1. 0 1 2 5 \end{array}
$$

$$
\begin{array}{r c l} S _ {\frac {2}{8}} & = & e x p \left\{(. 0 1) \frac {2}{8} + (. 1 5) W _ {\frac {2}{8}} \right\} \\ & = & e x p \left\{(. 0 1) \frac {2}{8} + (. 1 5) (-. 2 7 2 2) \right\} \approx . 9 5 9 7 \\ S _ {\frac {3}{8}} & = & e x p \left\{(. 0 1) \frac {3}{8} + (. 1 5) W _ {\frac {3}{8}} \right\} \\ & = & e x p \left\{(. 0 1) \frac {3}{8} + (. 1 5) (-. 5 3 4 5) \right\} \approx . 9 2 2 5 \\ S _ {\frac {4}{8}} & = & e x p \left\{(. 0 1) + (. 1 5) W _ {\frac {4}{8}} \right\} \\ & = & e x p \left\{(. 0 1) \frac {4}{8} + (. 1 5) (-. 1 5 1 9) \right\} \approx . 9 7 6 9 \\ S _ {\frac {5}{8}} & = & e x p \left\{(. 0 1) \frac {5}{8} + (. 1 5) W _ {\frac {5}{8}} \right\} \\ & = & e x p \left\{(. 0 1) \frac {5}{8} + (. 1 5) (-. 1 9 8 4) \right\} \approx . 9 6 9 9 \\ S _ {\frac {6}{8}} & = & e x p \left\{(. 0 1) \frac {6}{8} + (. 1 5) W _ {\frac {6}{8}} \right\} \\ & = & e x p \left\{(. 0 1) \frac {6}{8} + (. 1 5) (-. 0 6 0 5) \right\} \approx . 9 9 0 0 \\ S _ {\frac {7}{8}} & = & e x p \left\{(. 0 1) \frac {7}{8} + (. 1 5) W _ {\frac {7}{8}} \right\} \\ & = & e x p \left\{(. 0 1) \frac {7}{8} + (. 1 5) (-. 0 2 9 4) \right\} \approx . 9 9 4 5 \\ S _ {1} & = & e x p \left\{(. 0 1) \frac {1}{1} + (. 1 5) W _ {1} \right\} \\ & = & e x p \left\{(. 0 1) \frac {1}{1} + (. 1 5) (-. 2 5 4 1) \right\} \approx . 9 6 1 4 \end{array}
$$


Stock Price Path


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5882bd1f-b733-4ed9-8bdc-4c98ae290af0/07b17d5ae290b859c4baecaefc07b3ce5f14005f04474a46e71e903211fed024.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5882bd1f-b733-4ed9-8bdc-4c98ae290af0/75ae84a15756941b4bcedf73b611476d96c290531b000f7a5f2aade9036033a3.jpg)



FIGURE 0.10 Brownian Motion and Stock Price Paths


(c) What is the distribution of $\log \left(\frac{S_t}{S_{t - \Delta}}\right)$ ? With $S_0 = 1$ , $\log (S_t) = \mu t + \sigma W_t$ . 

$$
\begin{array}{r c l} \log \left(\frac {S _ {t}}{S _ {t - \Delta}}\right) & = & \log (S _ {t}) - \log (S _ {t - \Delta}) \\ & = & \mu t + \sigma W _ {t} - \mu (t - \Delta) - \sigma W _ {t - \Delta} \\ & = & \mu \Delta + \sigma (W _ {t} - W _ {t - \Delta}) \\ & = & \mu \Delta + \sigma W _ {\Delta} \\ & \stackrel {d} {\sim} & \mathcal {N} (\mu \Delta , \sigma^ {2} \Delta) \end{array}
$$

where $\mathcal{N}(\mu\Delta,\sigma^{2}\Delta)$ represents the normal distribution with mean $\mu\Delta$ and variance $\sigma^{2}\Delta$ . Therefore, log changes in the stock price over an increment of time $\Delta$ are normally distributed with mean $\mu\Delta$ and variance $\sigma^{2}\Delta$ . Note that the mean and variance are linear in time $\Delta$ . 

(d) The unit of measurement represents the log stock return. This random variable is distributed $\mathcal{N}(.25\mu,.25\sigma^{2})$ . 

(e) The random variable becomes distributed as a $\mathcal{N}(.000001\mu, .000001\sigma^2)$ . 

(f) Since $\mathcal{N}(\mu \Delta, \sigma^2\Delta)$ is equivalent to $\Delta \mathcal{N}(\mu, \frac{\sigma^2}{\Delta})$ , a problem arises since the variance explodes as $\Delta \to 0$ . The mean and variance are not “balanced” as would be the case if the distribution were $\mathcal{N}(\mu \Delta, \sigma^2\Delta^2)$ instead. 

(g) Brownian motion is not differentiable as $dW_{t}$ is a formalism. Therefore, the random variable is not well defined. 

## CHAPTER8

Since $\left(1 - \frac{\lambda}{n}\right)^k\to 1$ and $\left(1 - \frac{\lambda}{n}\right)^n\rightarrow e^{-\lambda}$ , it follows that 

$$
\begin{array}{r c l}P r (X _ {n} = k)&=&\binom {n} {k} \left(\frac {\lambda}{n}\right) ^ {k} \left(1 - \frac {\lambda}{n}\right) ^ {n - k}\\&=&\frac {\lambda^ {k}}{k !} \left(1 - \frac {\lambda}{n}\right) ^ {n} \left[ \frac {n (n - 1) \cdot \cdot \cdot (n - k + 1)}{n ^ {k}} \frac {1}{\left(1 - \frac {\lambda}{n}\right) ^ {k}} \right]\\&\rightarrow&\frac {\lambda^ {k}}{k !} e ^ {- \lambda}\end{array}
$$

as the contents of [ ] converges to 1. Therefore 

$$
P r (X _ {n} = k) \rightarrow \frac {\lambda^ {k} e ^ {- \lambda}}{k !}
$$

which is the density function for the Poisson distribution. 

(d) The probability of an event occurring decreases but the number of trials from which an event can occur increases. This is the central idea of insurance. Many people are insured with any individual having a small probability of an accident. 

## CHAPTER9

1. Calculate the stochastic integral $\int_0^t W_s^2 dW_s$ using Riemann and Ito integrals. 

(a) Three Riemann sums will differ according to the time-point at which the integrand is evaluated. Three possible choices are left, right, and middle of the partition as follows 

(1) 

$$
\sum_ {i = 1} ^ {n} W _ {i} ^ {2} \left(W _ {i} - W _ {i - 1}\right)\tag{2}
$$

$$
\sum_ {i = 1} ^ {n} W _ {i - 1} ^ {2} \left(W _ {i} - W _ {i - 1}\right)\tag{3}
$$

$$
\sum_ {i = 1} ^ {n} \left(\frac {W _ {i} + W _ {i - 1}}{2}\right) ^ {2} (W _ {i} - W _ {i - 1})
$$

(b) The Ito sum is represented by integral (2), $\sum_{i=1}^{n} W_{i-1}^2 (W_i - W_{i-1})$ . Integral (3) is known as a Stratonovich integral. 

(c) Expectations of the three integrals. The Ito integral, number (2), is zero since $W_{i-1}^2 \perp W_i - W_{i-1}$ by the property of independent increments for Brownian motion. 

$$
\begin{array}{r l r} {E \left[ \sum_ {i = 1} ^ {n} W _ {i - 1} ^ {2} (W _ {i} - W _ {i - 1}) \right]} & = & {\sum_ {i = 1} ^ {n} E [ W _ {i - 1} ^ {2} ] E [ (W _ {i} - W _ {i - 1}) ]} \\ & = & {\sum_ {i = 1} ^ {n} t _ {i - 1} 0} \\ & = & {0} \end{array}
$$

Integral (1) is also zero. 

$$
E \left[ \sum_ {i = 1} ^ {n} W _ {i} ^ {2} \left(W _ {i} - W _ {i - 1}\right) \right] = \sum_ {i = 1} ^ {n} \left(E \left[ W _ {i} ^ {3} \right] - E \left[ W _ {i} ^ {2} W _ {i - 1} \right]\right)
$$

$$
\begin{array}{r l} {=} & {- \sum_ {i = 1} ^ {n} E \left[ W _ {i} ^ {2} W _ {i - 1} \right]} \\ {=} & {- \sum_ {i = 1} ^ {n} E \left[ E \left[ W _ {i} ^ {2} W _ {i - 1} \big | \mathcal {I} _ {i - 1} \right] \right]} \\ {=} & {- \sum_ {i = 1} ^ {n} E \left[ W _ {i - 1} E \left[ W _ {i} ^ {2} \big | \mathcal {I} _ {i - 1} \right] \right]} \\ {=} & {- \sum_ {i = 1} ^ {n} E \left[ W _ {i - 1} \left(W _ {i - 1} ^ {2} + (t _ {i} - t _ {i - 1})\right) \right]} \\ {=} & {- \sum_ {i = 1} ^ {n} E \left[ W _ {i - 1} ^ {3} \right] - \sum_ {i = 1} ^ {n} (t _ {i} - t _ {i - 1}) E \left[ W _ {i - 1} \right]} \\ {=} & {0} \end{array}
$$

The term $E\left[W_{i}^{3}\right]=0$ since $W_{t}$ has a normal distribution which is symmetric. Therefore, all odd moments are zero. The value of the integral is calculated in closed form using results from chapter 11, problem 1. 

$$
\begin{array}{r c l} \int_ {0} ^ {t} W _ {2} ^ {2} d W _ {s} & = & \frac {W _ {t} ^ {3}}{3} - t W _ {t} + \int_ {0} ^ {t} s d W _ {s} \\ E \left[ \int_ {0} ^ {t} W _ {2} ^ {2} d W _ {s} \right] & = & E \left[ \frac {W _ {t} ^ {3}}{3} - t W _ {t} + \int_ {0} ^ {t} s d W _ {s} \right] \\ & = & E \left[ \frac {W _ {t} ^ {3}}{3} \right] \\ & = & 0 \end{array}
$$

The integral $\int_{0}^{t} sdW_{s}$ has zero expectation as it is a well defined Ito integral. Integral (3) is an “average” of the previous two integrals and therefore has an expected value equal to zero. Overall, this example should not form the impression that the choice of integrand is irrelevant. For instance, consider the integral $\int_{0}^{t} W_{s} dW_{s}$ and two seemingly similar integrands, one of which uses $W_{i-1}$ and the other $W_{i}$ as the integrand in the approximation. A major difference reveals itself. 

Ito Representation 

$$
\begin{array}{r l r} {\sum_ {i = 1} ^ {n} W _ {i - 1} \left(W _ {i} - W _ {i - 1}\right)} & \\ {E \left[ \sum_ {i = 1} ^ {n} W _ {i - 1} \left(W _ {i} - W _ {i - 1}\right) \right]} & = & {\sum_ {i = 1} ^ {n} E \left[ W _ {i - 1} \right] E \left[ \left(W _ {i} - W _ {i - 1}\right) \right]} \\ & = & {0} \end{array}
$$

Non Ito Representation 

$$
\begin{array}{r c l} \sum_ {i = 1} ^ {n} W _ {i} (W _ {i} - W _ {i - 1}) & = & \sum_ {i = 1} ^ {n} (W _ {i} - W _ {i - 1}) (W _ {i} - W _ {i - 1}) + \sum_ {i = 1} ^ {n} W _ {i - 1} (W _ {i} - W _ {i - 1}) \\ E [ \sum_ {i = 1} ^ {n} W _ {i} (W _ {i} - W _ {i - 1}) ] & = & \sum_ {i = 1} ^ {n} E [ (W _ {i} - W _ {i - 1}) ^ {2} ] + 0 \\ & = & t \end{array}
$$

Where the last result follows from the definition of quadratic variation and the previous result for the Ito integral. 

(d) The Ito integral has zero expectation as was noted above. 

## 2. Integration by Parts

Show that $\sum_{j = 1}^{n}\left[t_jW_{t_j} - t_{j - 1}W_{t_{j - 1}}\right] = \sum_{j = 1}^{n}\left[t_j\left(W_{t_j} - W_{t_{j - 1}}\right)\right] + \sum_{j = 1}^{n}\left[\left(t_j - t_{j - 1}\right)W_{t_{j - 1}}\right].$ 

The sum on the left hand side is a telescoping sum which reduces to 

$$
\begin{array}{r l} & {\sum_ {j = 1} ^ {n} \left[ t _ {j} W _ {t _ {j}} - t _ {j - 1} W _ {t _ {j - 1}} \right]} \\ {=} & {t _ {1} W _ {t _ {1}} - t _ {0} W _ {t _ {0}} + t _ {2} W _ {t _ {2}} - t _ {1} W _ {t _ {1}} + \ldots + t _ {n} W _ {t _ {n}} - t _ {n - 1} W _ {t _ {n - 1}}} \\ {=} & {t _ {n} W _ {t _ {n}} - t _ {0} W _ {t _ {0}}} \\ {=} & {t W _ {t}} \end{array}
$$

as $t_{n}=t$ and $W_{t_{0}}=W_{0}=0$ . The right hand side is also a telescoping sum. 

$$
\begin{array}{r l} & {\sum_ {j = 1} ^ {n} \left[ t _ {j} \left(W _ {t _ {j}} - W _ {t _ {j - 1}}\right) \right] + \sum_ {j = 1} ^ {n} \left[ (t _ {j} - t _ {j - 1}) W _ {t _ {j - 1}} \right]} \\ {=} & {t _ {1} W _ {t _ {1}} - t _ {1} W _ {t _ {0}} + t _ {1} W _ {t _ {0}} - t _ {0} W _ {t _ {0}} + t _ {2} W _ {t _ {2}} - t _ {2} W _ {t _ {1}} + t _ {2} W _ {t _ {1}} - t _ {1} W _ {t _ {1}} + \ldots} \\ & {+ t _ {n} W _ {t _ {n}} - t _ {n} W _ {t _ {n - 1}} + t _ {n} W _ {t _ {n - 1}} - t _ {n - 1} W _ {t _ {n - 1}}} \\ {=} & {t _ {n} W _ {t _ {n}} - t _ {0} W _ {t _ {0}}} \\ {=} & {t W _ {t}} \end{array}
$$

In this example, with only one process being stochastic, the above does represent the standard product rule. Let $u(t) = t$ and $v(t) = W_{t}$ . An extra term would account for the quadratic variation if the integrand and integrator were both semimartingales (see below). 

3. In the limit, as the partition width goes to zero 

$$
\begin{array}{r c l} t W _ {t} & = & \int_ {0} ^ {t} s d W _ {s} + \int_ {0} ^ {t} W _ {s} d s \\ \Rightarrow \int_ {0} ^ {t} s d W _ {s} & = & t W _ {t} - \int_ {0} ^ {t} W _ {s} d s \end{array}
$$

4. The integral $\int_0^t sdW_s$ is defined in the sense of the Ito integral. 

5. This is not a change of variable formula. 

6. Problem 3 is an example of integration by parts. In general, when $u(t)$ and $v(t)$ are both stochastic semimartingales 

$$
u (t) v (t) = u (0) v (0) + \int_ {0} ^ {t} u (s) d v (s) + \int_ {0} ^ {t} v (s) d u (s) + \langle u (s), v (s) \rangle_ {t}
$$

where $\langle \cdot, \cdot \rangle_t$ represents the quadratic variation of the two processes. When at least one of the two processes is of bounded variation, the quadratic variation is zero. In this case, the formula reduces to 

$$
\begin{array}{r c l} u (t) v (t) & = & u (0) v (0) + \int_ {0} ^ {t} u (s) d v (s) + \int_ {0} ^ {t} v (s) d u (s) \\ \Rightarrow d (u (t) v (t)) & = & u (t) d v (t) + v (t) d u (t) \end{array}
$$

## CHAPTER 10

1. Differentiate the following functions using Ito's lemma. 

$$
\begin{array}{r l r} {d f (W _ {t})} & = & {f ^ {\prime} (W _ {t}) d W _ {t} + \frac {1}{2} f ^ {\prime \prime} (W _ {t}) d t} \\ {d f (W _ {t}, t)} & = & {f _ {t} (W _ {t}, t) d t + f ^ {\prime} (W _ {t}, t) d W _ {t} + \frac {1}{2} f ^ {\prime \prime} (W _ {t}, t) d t} \end{array}
$$

(a) $f(W_{t}) = W_{t}^{2}$ 

$$
d f (W _ {t}) = 2 W _ {t} d W _ {t} + d t
$$

$$
f (W _ {t}) = W _ {t} ^ {\frac {1}{2}}
$$

$$
d f (W _ {t}) = \frac {1}{2} W _ {t} ^ {- \frac {1}{2}} d W _ {t} - \frac {1}{8} W _ {t} ^ {- \frac {3}{2}} d t
$$

(b) $f(W_{t}) = e^{W_{t}^{2}}$ 

$$
\begin{array}{r c l} {f ^ {\prime} (W _ {t})} & = & {2 W _ {t} e ^ {W _ {t} ^ {2}}} \\ {f ^ {\prime \prime} (W _ {t})} & = & {2 e ^ {W _ {t} ^ {2}} + 4 W _ {t} ^ {2} e ^ {W _ {t} ^ {2}}} \\ {\Rightarrow d f (W _ {t})} & = & {2 W _ {t} e ^ {W _ {t} ^ {2}} d W _ {t} + \left[ e ^ {W _ {t} ^ {2}} + 2 W _ {t} ^ {2} e ^ {W _ {t} ^ {2}} \right] d t} \end{array}
$$

(c) $f(W_{t}, t) = e^{\left(\sigma W_{t} - \frac{1}{2}\sigma^{2}t\right)}$ 

$$
{\frac {\partial f (W _ {t} , t)}{\partial t}} = {- \frac {1}{2} \sigma^ {2} f (W _ {t}, t)}
$$

$$
\begin{array}{r c l} \frac {\partial f (W _ {t} , t)}{\partial W _ {t}} & = & \sigma f (W _ {t}, t) \\ \frac {\partial^ {2} f (W _ {t} , t)}{\partial^ {2} W _ {t}} & = & \sigma^ {2} f (W _ {t}, t) \\ \Rightarrow d f (W _ {t}, t) & = & f (W _ {t}, t) \left[ \left(- \frac {1}{2} \sigma^ {2} + \frac {1}{2} \sigma^ {2}\right) d t + \sigma d W _ {t} \right] \\ & = & \sigma f (W _ {t}, t) d W _ {t} \end{array}
$$

$$
f (W _ {t}, t) = e ^ {\sigma W _ {t}}
$$

Similar to above except that $\frac{\partial f(W_{t},t)}{\partial t}=0$ . This implies that a drift term is introduced and the process is no longer a martingale as in the previous case. 

$$
d f (W _ {t}) = \frac {1}{2} \sigma^ {2} f (W _ {t}) d t + \sigma f (W _ {t}) d W _ {t}
$$

(d) $g(t) = \int_{0}^{t} W_{s} ds$ 

$$
\frac {\partial g (t)}{\partial t} = W _ {t} d t
$$

2. Obtain SDE's for processes below involving $W_{t}^{1}$ and $W_{t}^{2}$ . The 1 and 2 are superscripts, not exponents which are denoted with brackets. 

(a) $dX_{t} = 4\left(W_{t}^{1}\right)^{3}dW_{t}^{1} + 6\left(W_{t}^{1}\right)^{2}dt$ 

(b) $X_{t} = \left(W_{t}^{1} + W_{t}^{2}\right)^{2}$ The term $\left\langle W_{s}^{1}, W_{s}^{2} \right\rangle_{t} = \left\langle W_{s}^{2}, W_{s}^{1} \right\rangle_{t}$ is the “covariance” between the two Brownian motions which equals zero if the two Brownian motions are independent. 

$$
\begin{array}{r c l}\frac {\partial X _ {t}}{\partial W _ {t} ^ {1}}&=&\frac {\partial X _ {t}}{\partial W _ {t} ^ {2}} = 2 \left(W _ {t} ^ {1} + W _ {t} ^ {2}\right)\\\frac {\partial^ {2} X _ {t}}{\partial^ {2} W _ {t} ^ {1}}&=&\frac {\partial^ {2} X _ {t}}{\partial^ {2} W _ {t} ^ {2}} = \frac {\partial^ {2} X _ {t}}{\partial W _ {t} ^ {1} \partial W _ {t} ^ {2}} = 2\\\Rightarrow d X _ {t}&=&\frac {1}{2} \left[ (2 + 2) d t + (2 + 2) \left<   W _ {s} ^ {1}, W _ {s} ^ {2} \right> _ {t} \right] d t + 2 \left(W _ {t} ^ {1} + W _ {t} ^ {2}\right)\left(d W _ {t} ^ {1} + d W _ {t} ^ {2}\right)\\&=&2 \left[ 1 + \left<   W _ {s} ^ {1}, W _ {s} ^ {2} \right> _ {t} \right] d t + 2 \left(W _ {t} ^ {1} + W _ {t} ^ {2}\right)\left(d W _ {t} ^ {1} + d W _ {t} ^ {2}\right)\end{array}
$$

(c) $X_{t} = t^{2} + e^{W_{t}^{2}}$ 

$$
\begin{array}{r c l} \frac {\partial X _ {t}}{\partial t} & = & 2 t \\ \frac {\partial X _ {t}}{\partial W _ {t} ^ {2}} & = & \frac {\partial^ {2} X _ {t}}{\partial^ {2} W _ {t} ^ {2}} = e ^ {W _ {t} ^ {2}} \\ \Rightarrow d X _ {t} & = & \left(2 t + \frac {1}{2} e ^ {W _ {t} ^ {2}}\right) d t + e ^ {W _ {t} ^ {2}} d W _ {t} ^ {2} \end{array}
$$

(d) $X_{t} = e^{t^{2} + W_{t}^{2}}$ 

$$
{\frac {\partial X _ {t}}{\partial t}} = {2 t X _ {t}}
$$

$$
{\frac {\partial X _ {t}}{\partial W _ {t} ^ {2}}} = {\frac {\partial^ {2} X _ {t}}{\partial^ {2} W _ {t} ^ {2}} = X _ {t}}
$$

$$
\Rightarrow d X _ {t} = \left(2 t + \frac {1}{2}\right) X _ {t} d t + X _ {t} d W _ {t} ^ {2}
$$

3. Geometric Brownian motion, $S_{t} = S_{0} e^{\left( \mu - \frac{1}{2} \sigma^{2} \right) t + \sigma W_{t}}$ 

(a) $dS_{t} = \mu S_{t}dt + \sigma S_{t}dW_{t}$ which follows from Ito's lemma (see problem 1, part (c) above) 

$$
{S (W _ {t}, t)} = {S (W _ {0}, 0) e ^ {\mu t + \sigma W _ {t} - \frac {1}{2} \sigma^ {2} t}}
$$

$$
{\frac {\partial S (W _ {t} , t)}{\partial t}} = {\mu S (W _ {t}, t) - \frac {1}{2} \sigma^ {2} S (W _ {t}, t)}
$$

$$
{\frac {\partial S (W _ {t} , t)}{\partial W _ {t}}} = {\sigma S (W _ {t}, t)}
$$

$$
{\frac {\partial^ {2} S (W _ {t} , t)}{\partial^ {2} W _ {t}}} = {\sigma^ {2} S (W _ {t}, t)}
$$

$$
\begin{array}{r l r} \Rightarrow d S (W _ {t}, t) & = & S (W _ {t}, t) \left[ \left(\mu - \frac {1}{2} \sigma^ {2} + \frac {1}{2} \sigma^ {2}\right) d t + \sigma d W _ {t} \right] \\ & = & \mu S (W _ {t}, t) d t + \sigma S (W _ {t}, t) d W _ {t} \end{array}
$$

$$
{\frac {d S _ {t}}{S _ {t}}} = {\mu d t + \sigma d W _ {t}}
$$

(b) The expected instantaneous rate of change is the drift rate, $\mu$ . 

(c) Without the term $-\frac{1}{2}\sigma^2 t$ in the exponent, the dynamics of $S_{t}$ would be 

$$
\frac {d S _ {t}}{S _ {t}} = \left(\mu + \frac {1}{2} \sigma^ {2}\right) d t + \sigma d W _ {t}
$$

There is no cancellation of the $\frac{1}{2}\sigma^2$ term by the partial derivative with respect to time. Now, the expected rate of change is $\mu +\frac{1}{2}\sigma^2$ under the empirical measure. 

## CHAPTER 11

1. Consider the SDE $d(W_t^3) = 3\left[W_tdt + W_t^2 dW_t\right]$ 

(a) Write the SDE in integral format. 

$$
\begin{array}{r c l} W _ {t} ^ {3} & = & W _ {0} ^ {3} + 3 \int_ {0} ^ {t} W _ {s} d s + 3 \int_ {0} ^ {t} W _ {s} ^ {2} d W _ {s} \\ & = & 3 \int_ {0} ^ {t} W _ {s} d s + 3 \int_ {0} ^ {t} W _ {s} ^ {2} d W _ {s} \end{array}
$$

(b) Evaluate $\int_0^t W_s^2 dW_s$ . Certain results follow from chapter 9, problem 1. From the above equation 

$$
\begin{array}{r c l} \int_ {0} ^ {t} W _ {s} ^ {2} d W _ {s} & = & \frac {W _ {t} ^ {3}}{3} - \int_ {0} ^ {t} W _ {s} d s \\ & = & \frac {W _ {t} ^ {3}}{3} - \left[ t W _ {t} - \int_ {0} ^ {t} s d W _ {s} \right] \mathrm{fromchapter9} \\ & = & \frac {W _ {t} ^ {3}}{3} - t W _ {t} + \int_ {0} ^ {t} s d W _ {s} \end{array}
$$

The integral $\int_0^t sdW_s$ is normally distributed with mean zero and variance $\int_0^t s^2 ds = \frac{t^3}{3}$ . The random variable $\mathcal{N}\left(0,\frac{t^3}{3}\right)$ could be represented as a time changed Brownian motion, $W_{\frac{t^3}{3}}$ . 

$$
\int_ {0} ^ {t} W _ {2} ^ {2} d W _ {s} = \frac {W _ {t} ^ {3}}{3} - t W _ {t} + W _ {\frac {t ^ {3}}{3}}
$$

$$
2. d S _ {t} = \mu S _ {t} d t + \sigma S _ {t} d W _ {t} \Rightarrow S (t) = S (0) e x p \left\{\mu t + \sigma W _ {t} - \frac {1}{2} \sigma^ {2} t \right\}
$$

(a) Coin tossing to approximate $dW_{t} \approx \Delta W_{t}$ 

$$
\Delta W _ {t} = \left\{ \begin{array}{l l} + \sqrt {\Delta} & \mathrm{ifcointossisheads.5probability} \\ - \sqrt {\Delta} & \mathrm{ifcointossistails.5probability} \end{array} \right.
$$

(b) $\Delta W$ is distributed with zero mean and variance $\Delta$ . The above in part (a) is a binomial distribution with probability $\frac{1}{2}$ which has the same mean and variance as $\Delta W_{t}$ . 

$$
\begin{array}{r l} \mathrm{mean} & \frac {1}{2} (\sqrt {\Delta}) + \frac {1}{2} (- \sqrt {\Delta}) = 0 \\ \mathrm{variance} & \frac {1}{2} (\sqrt {\Delta}) ^ {2} + \frac {1}{2} (- \sqrt {\Delta}) ^ {2} = \Delta \end{array}
$$

(c) Generate three random paths over the 8 day period in 2 day increments $(\Delta = 2)$ . Must flip 4 coins to determine a path. 

$$
S (t + 2) = S (t) e ^ {. 0 7 7 5 + (. 1 5) \Delta W}
$$

The amount .0775 follows from the drift (where the drift is equal to the risk - free interest rate), $(2)(.05)-\frac{1}{2}(2)(.15)^{2}$ . These simulations are under the equivalent risk - neutral martingale measure as stock's drift rate is the risk - free interest rate. A MATLAB program below replaces the act of tossing a coin with a draw from the binomial distribution. 

```matlab
%number of simulations
m=3;
%number of draws (nodes) per simulation
n=4;
stock=zeros(m,n+1);
stock(:,1)=940;

for j=1:m
    for i=2:n+1
    x=binornd(1,.5); %x is either 1 (heads) or 0 (tails)
    if x==1
    delW = sqrt(2);
    else
    delW = -sqrt(2);
    end
    stock(j,i)=stock(j,i-1)*exp(.0775 + .15 * delW);
    end
end

%path 1
stock(1,)
940 821.60 1097.60 959.34 1281.62
%path 2
stock(2,)
940 821.60 718.12 959.34 1281.62
%path 3
stock(3,:) 
```

3. $dS_{t} = .01S_{t}dt + .05S_{t}dW_{t}$ 

(a) see MATLAB program below 

(b) see MATLAB program below 

(c) A MATLAB program below generates 5 normally distributed random variables with mean 0 and variance .20, then computes the stock price and call value. 

```matlab
sigma = .05;
T = 1;
K = 1;
r = .03;
SO = 1;

%n is the number of discretizations for T
n = 5;
delta = T/n;

bm(1)=normrnd(0,sqrt(delta));
cbm(1) = bm(1);

for j=2:n
    bm(j) = normrnd(0,sqrt(delta));
    cbm(j) = cbm(j-1) + bm(j);
end

for j=1:n
    stock(j) = SO*exp((r*j*delta)+sigma*cbm(j)-(1/2)*(sigma^2)*j*delta);
end

%generate European call price
%stock(n) is final stock price, stock(T)
call = exp(-r*T) * max(0, stock(n) - K)

0.0312 <- call value (one simulation)

stock

0.9980 1.0162 1.0447 1.0510 1.0321 <- one possible stock price path 
```

(d) Need parameters for a uniform distribution with mean 0 and variance $\frac{1}{5}$ . Since the parameters must generate a symmetric distribution with mean zero, $a = -b$ . To ensure that the variance equals $\frac{1}{5}$ , choose $b$ such that 

$$
\begin{array}{r c l} \frac {1}{5} & = & \frac {(b - a) ^ {2}}{1 2} \\ & = & \frac {(2 b) ^ {2}}{1 2} \\ & = & \frac {b ^ {2}}{3} \end{array}
$$

$$
\begin{array}{r c l} \Rightarrow \frac {3}{5} & = & b ^ {2} \\ \Rightarrow b & = & \sqrt {. 6} \end{array}
$$

Therefore, draw the random variables from a uniform distribution, $\mathcal{U}(-\sqrt{.6},\sqrt{.6})$ . A MATLAB program which performs these calculations is given below. 

```matlab
sigma = .05;
T = 1;
K = 1;
r = .03;
SO = 1;

%n is the number of discretizations for T
n = 5;
delta = T/n;

bm(1)=unifrnd(-sqrt(.6),sqrt(.6));
cbm(1) = bm(1);

for j=2:n
    bm(j) = unifrnd(-sqrt(.6),sqrt(.6));
    cbm(j) = cbm(j-1) + bm(j);
end

for j=1:n
    stock(j) = S0*exp((r*j*delta)+sigma*cbm(j)-(1/2)*(sigma^2)*j*delta);
end

%generate European call price
%stock(n) is final stock price, stock(T)
call = exp(-r*T) * max(0, stock(n) - K)

0.0353 <- call value (one simulation)

stock

1.0193 1.0523 1.0198 1.0401 1.0364 <- one possible stock price path 
```

(e) Repeat the experiment 1,000 times and compare the two approximation methods. 

```matlab
%generates Brownian motion using Normal and Uniform approximations, then generates
%stock prices and European call values (1000 times)
for k=1:1000
sigma = .05;
T = 1;
K = 1;
r = .03;
S0 = 1;
%n is the number of discretizations for T
n = 5; 
```

```matlab
delta = T/n;

bm_normal(1)=normrnd(0,sqrt(delta));
cbm_normal(1) = bm_normal(1);
bm_uniform(1)=unifrnd(-sqrt(.6),sqrt(.6));
cbm_uniform(1) = bm_uniform(1);

for j=2:n
    bm_normal(j) = normrnd(0,sqrt(delta));
    cbm_normal(j) = cbm_normal(j-1) + bm_normal(j);
    bm_uniform(j) = unifrnd(-sqrt(.6),sqrt(.6));
    cbm_uniform(j) = cbm_uniform(j-1) + bm_uniform(j);
end

for j=1:n
    stock_normal(j) = S0*exp((r*j*delta)+sigma*cbm_normal(j)-(1/2)*(sigma^2)*j*delta);
    stock_uniform(j) = S0*exp((r*j*delta)+sigma*cbm_uniform(j)-(1/2)*(sigma^2)*j*delta);
end

%generate European call price
%stock(n) is final stock price, stock(T)
call_normal(k) = exp(-r*T) * max(0, stock_normal(n) - K);
call_uniform(k) = exp(-r*T) * max(0, stock_uniform(n) - K);

end

avgnormal=mean(call_normal)

0.0381 <- call value using Normal approximation

avguniform=mean(call_uniform)

0.0388 <- call value using Binomial approximation 
```

The two prices are similar. In general, the central limit theorem could be invoked if n were increased. The sum of independent uniform random variables with a common mean converges to a normal distribution. 

Note: MATLAB has a built in Black Scholes option pricing formula (among many other finance related features). 

(f) Yes, the paths may be combined. However, the accuracy of the expectation also depends on the number of nodes in the sample path and not just the number of sample paths. Rather than combine simulations (increase k), decreasing the partition width (increase n) would be more suitable. There are two sources of error, one arises from the discretization and the other from the Monte Carlo simulation for a given discretization. With only five nodes in the discretization, the central limit theorem cannot be invoked. Increasing the number k of simulated paths simply makes the sample average approach the expected call value calculated with only five nodes, this is not the true call value. 

4. Consider the process $dS_{t} = .05dt + .1dW_{t}$ . This is arithmetic and not geometric Brownian motion. The terms $dW_{t}$ are approximated by 

$$
\Delta W _ {t} = \left\{ \begin{array}{l l} + \sqrt {\Delta} & \mathrm{withprobability.5} \\ - \sqrt {\Delta} & \mathrm{withprobability.5} \end{array} \right.
$$

(a) see MATLAB program below 

(b) see MATLAB program below 

(c) Stock price path plots with $\Delta = 1$ and $\Delta = .5$ . 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5882bd1f-b733-4ed9-8bdc-4c98ae290af0/5e564ac640db9300182f374b889f12607e3d0ecf987ade59e7416b5a0cf3989e.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5882bd1f-b733-4ed9-8bdc-4c98ae290af0/7e0dcf63d96f8729ef13700cfbce70f92d056bc3b0f1a890e588598321f2a4cc.jpg)



FIGURE 0.11 Stock Price Paths


(d) A MATLAB program is presented below with draws from a binomial distribution to simulate coin tossing. For $\Delta = 1$ , choose n to be 3, for $\Delta = .5$ , choose n to be 6, and for $\Delta = .01$ , choose n to be $\frac{3}{.01} = 300$ . 

```matlab
n=[3,6,300];
stock(1)=1;
sig=.1;

for j=1:3
    delta=3/n(j);
    for i=2:n(j)+1
    %x is either 1 (heads) or 0 (tails)
    x=binornd(1,.5);
    if x==1
    delW = sqrt(delta);
    else
    delW = -sqrt(delta);
    end
    stock(i)=stock(i-1) + .05 * delta + sig * delW;
    end
    x=[0:delta:3];
    plot(x,stock)
    title('Path of Stock Price')
    xlabel('Time') 
```

%pause command will generate plot and wait for return key to proceed pause 

As the plots indicate, when $\Delta = .01$ , the stock price process looks as if it is being driven by a Brownian motion. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5882bd1f-b733-4ed9-8bdc-4c98ae290af0/fbc45afde2b00ae06bf756b2b096430a6340bbbed3782f27fc55e3928ca817f5.jpg)



Path of Stock Price, Delta = .01, sigma=.1*sqrt(3)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5882bd1f-b733-4ed9-8bdc-4c98ae290af0/2ce79576e8a9ebeacf689e6e469ec56be4e6aa5aa484811806930c7596eefaf4.jpg)



FIGURE 0.12 Stock Price Paths


(e) To increase the variance by a factor of 3, change $\sigma$ from .10 to $\sqrt{3}(.10)$ . After this value is adjusted in the above MATLAB program, new plots are generated. One possible path is 1.0000 1.2232 1.4464 1.3232 <- one possible stock price path 

## CHAPTER 12

1. Laplace's equation: $f_{xx} + f_{yy} + f_{zz} = 0$ . Is Laplace's equation satisfied by the following equations? 

(a) $f(x,z,y)=4z^{2}y-x^{2}y-y^{3}$ YES 

$$
\begin{array}{r l r} & & {f _ {x x} = - 2 y \qquad f _ {y y} = - 6 y \qquad f _ {z z} = 8 y} \\ & {\Rightarrow} & {f _ {x x} + f _ {y y} + f _ {z z} = 0} \end{array}
$$

(b) $f(x, y) = x^{2} - y^{2}$ YES 

$$
\begin{array}{r l} & f _ {x x} = 2 \qquad f _ {y y} = - 2 \\ \Rightarrow & f _ {x x} + f _ {y y} = 0 \end{array}
$$

(c) $f(x, y) = x^{3} - 3xy$ NO 

$$
\begin{array}{r l r} & & {f _ {x x} = 6 x \qquad f _ {y y} = 0} \\ & {\Rightarrow} & {f _ {x x} + f _ {y y} = 6 x \neq 0 \forall x} \end{array}
$$

(d) $f(x,z,y)=\frac{x}{y+z}$ NO 

$$
\begin{array}{r c l} f _ {x} & = & \frac {1}{y + z} \Rightarrow f _ {x x} = 0 \\ f _ {y} & = & \frac {- x}{(y + z) ^ {2}} \Rightarrow f _ {y y} = \frac {2 x}{(y + z) ^ {3}} \\ f _ {z} & = & \frac {- x}{(y + z) ^ {2}} \Rightarrow f _ {z z} = \frac {2 x}{(y + z) ^ {3}} \\ \Rightarrow f _ {x x} + f _ {y y} + f _ {z z} & = & \frac {4 x}{(y + z) ^ {3}} \neq 0 \forall x \end{array}
$$

More than one function will satisfy Laplace's equation unless boundary conditions are specified. The number of boundary conditions depends on the domain. Boundary conditions are needed as one can always add constants and terms of the form x, y,, and xy without changing the second derivative. Boundary conditions serve a purpose similar to initial conditions in ordinary differential equations. A unique solution is desirable when all necessary boundary conditions have been specified. 

2. Do the following functions satisfy the heat equation? 

$$
\mathrm{(a)} f (x, z, y) = e ^ {\left[ 2 9 a ^ {2} \pi^ {2} t + \pi (3 x + 2 y + 4 z) \right]} \quad \mathrm{YES}
$$

$$
\begin{array}{r c l} \frac {\partial f (x , z , y)}{\partial t} & = & 2 9 a ^ {2} \pi^ {2} f (x, z, y) \\ \frac {\partial^ {2} f (x , z , y)}{\partial^ {2} x} & = & 9 \pi^ {2} f (x, z, y) \\ \frac {\partial^ {2} f (x , z , y)}{\partial^ {2} y} & = & 4 \pi^ {2} f (x, z, y) \\ \frac {\partial^ {2} f (x , z , y)}{\partial^ {2} z} & = & 1 6 \pi^ {2} f (x, z, y) \end{array}
$$

Therefore, $a^{2}$ times the sum of the second derivatives, $a^{2}\left(f_{xx} + f_{yy} + f_{zz}\right)$ equals $f_{t}$ and the heat equation is satisfied. 

$$
\begin{array}{r c l} {a ^ {2} (f _ {x x} + f _ {y y} + f _ {z z})} & = & {a ^ {2} (9 + 4 + 1 6) \pi^ {2} f (x, z, y)} \\ & = & {2 9 a ^ {2} \pi^ {2} f (x, z, y)} \\ & = & {f _ {t}} \end{array}
$$

$$
f (x, z, y) = 3 x ^ {2} + 3 y ^ {2} - 6 z ^ {2} + x + y - 9 z - 3 \quad \mathrm{YES}
$$

Since there is no dependence on t, this equation satisfies the heat equation if and only if it satisfies Laplace's equation as $f_{t} = 0$ . Only terms of quadratic order or higher need to be considered, $3x^{2} + 3y^{2} - 6z^{2}$ , as lower order terms vanish when the Laplacian is applied. 

$$
\begin{array}{r l} & f _ {x x} = 6 \qquad f _ {y y} = 6 \qquad f _ {z z} = - 1 2 \\ \Rightarrow \qquad & f _ {x x} + f _ {y y} + f _ {z z} = 0 \end{array}
$$

The heat equation is satisfied. 

3. PDE: $f_{x} + .2f_{y} = 0$ with $x \in [0, 1]$ and $y \in [0, 1]$ . 

(a) The function $f(x,y)$ is the unknown in the above equation. 

(b) $f_{y} = -5f_{x}$ . In English, a function such that the change in y is minus 5 times the change in x is required. 

(c) There will be infinitely many solutions to the equation without a boundary condition. For instance, consider the class of constant solutions, $f(x,y) = k$ where $k \in \mathcal{R}$ (any real number). In this instance, $f_{x} = f_{y} = 0$ and $f_{x} + .2f_{y} = 0$ as desired. In addition, $f(x,y) = -.2\lambda x + \lambda y$ and $f(x,y) = e^{\lambda (.2x - y)}$ can also be shown to satisfy the equation for any constant $\lambda \in \mathcal{R}$ . The PDE is the linear homogeneous transport equation and in general 

$$
\begin{array}{r c l} f _ {x} (x, y) +. 2 f _ {y} (x, y) & = & 0 \\ f (x, y) | _ {x = 0} & = & g (0, y) \end{array}
$$

has a solution $f(x,y) = g(y - .2x)$ . 

(d) Impose the boundary condition $f(0,y) = 1$ . The unique solution is $f(x,y) = 1$ since the function $g$ is identically 1. This corresponds the first class of solutions in part (c) when $k = 1$ . 

4. The PDE is the heat equation, $f_{xx} + .2f_t = 0$ , with boundary condition $f(x,1) = max[x - 6,0]$ for $0 \leq x \leq 12$ and $0 \leq t \leq 1$ . The boundary condition is for a European call option. 

(a) A single boundary condition is not sufficient, the rectangle (time by space) has four sides. Three boundary conditions must be specified. The fourth side, $f(x,0)$ , is then solved as the value of the option at the current date, $t = 0$ , for various initial stock prices. 

(b) Two reasonable assumptions for boundary conditions would be that $f(0, t) = 0$ and $f(12, t) = 6$ . The first boundary condition specifies that if the stock price becomes zero it stays zero. The second boundary condition states that when the option becomes very deep in-the-money, $6, it remains at that level. 

(c) Implement a numerical approximation using grid sizes of $\Delta x = 3$ and $\Delta t = .24$ . The simplest technique is an explicit scheme with a backward time derivative (more elaborate procedures would involve an implicit Crank - Nicholson scheme). Let k be the time horizon (0, .25, .50, .75, 1.0) and j be the state space (0, 3, 6, 9, 12). The numerical routine operates backward in time starting from k = 1 and proceed to k = 0, when the values of the function (call values) are known for a given initial stock price. At each step, the program will solve for $u_{j}^{k-1}$ as the k terms are known. 

$$
\begin{array}{r c l} \frac {u _ {j} ^ {k} - u _ {j} ^ {k - 1}}{\Delta t} & = & - 5 \left(\frac {u _ {j + 1} ^ {k} - 2 u _ {j} ^ {k} + u _ {j - 1} ^ {k}}{(\Delta x) ^ {2}}\right) \\ u _ {j} ^ {k} - u _ {j} ^ {k - 1} & = & - 5 \frac {\Delta t}{(\Delta x) ^ {2}} \left(u _ {j + 1} ^ {k} - 2 u _ {j} ^ {k} + u _ {j - 1} ^ {k}\right) \\ u _ {j} ^ {k - 1} & = & u _ {j} ^ {k} + \frac {5}{3 6} \left(u _ {j + 1} ^ {k} - 2 u _ {j} ^ {k} + u _ {j - 1} ^ {k}\right) \end{array}
$$

The MATLAB program below performs the calculations. 

```matlab
Matrix=zeros(5,5);
Matrix(:,5)=[6,6,6,6,6]';
Matrix(1,:)=[0,0,0,3,6];
for k=1:4
    for j=4:-1:2
    Matrix(k+1,j)=Matrix(k,j)+(5/36)*(Matrix(k,j+1)-2*Matrix(k,j)+Matrix(k,j-1));
    end
end 
```

For instance, to calculate the $(2,4)$ entry of $3, the following was done 

$$
x = 3 + \frac {5}{3 6} (6 - 2 (3) + 0) = 3
$$

The values at the various nodes can be seen from the final values of Matrix. 

Matrix = 

<table><tr><td>0</td><td>0</td><td>0</td><td>3.0000</td><td>6.0000</td></tr><tr><td>0</td><td>0</td><td>0.4167</td><td>3.0000</td><td>6.0000</td></tr><tr><td>0</td><td>0.0579</td><td>0.7176</td><td>3.0579</td><td>6.0000</td></tr><tr><td>0</td><td>0.1415</td><td>0.9510</td><td>3.1415</td><td>6.0000</td></tr><tr><td>0</td><td>0.2342</td><td>1.1428</td><td>3.2342</td><td>6.0000</td></tr></table>

To interpret the results, time to maturity is increasing down the rows and the value of x (initial stock price) is increasing from column to column (going right). Therefore the results are consistent with financial intuition. Prices increase along each column from left to right as the current stock price increases. Prices converge to their intrinsic value from the bottom to the top row as the “option” approaches maturity. Overall, the bottom row 

<table><tr><td>S(0)</td><td>$0</td><td>$3</td><td>$6</td><td>$9</td><td>$12</td></tr><tr><td>t=0</td><td>0</td><td>0.2342</td><td>1.1428</td><td>3.2342</td><td>6.0000</td></tr></table>


represents the current value of the “option” at various initial stock prices. 


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5882bd1f-b733-4ed9-8bdc-4c98ae290af0/853740e27c85a91a5d85af6a7969554925b7fb17d2c36c78b2f80dde1e67877d.jpg)



FIGURE 0.13 Numerical PDE Solution


## CHAPTER 13

1. $X_{t} = e^{Y_{t}}$ where $Y_{t}\sim \mathcal{N}(\mu t,\sigma^{2}t)$ 

(a) Calculate $E[X_t|X_s, s < t]$ 

$$
\begin{array}{r c l} E \left[ X _ {t} | X _ {s}, s <   t \right] & = & E \left[ e ^ {Y _ {t}} \mid Y _ {s}, s <   t \right] \\ & = & E \left[ e ^ {Y _ {t} - Y _ {s} + Y _ {s}} \mid Y _ {s}, s <   t \right] \\ & = & e ^ {Y _ {s}} E \left[ e ^ {Y _ {t} - Y _ {s}} \mid Y _ {s}, s <   t \right] \end{array}
$$

Since $Y_{s}$ is not random, the term $e^{Y_{s}}$ can be removed from under the expectation. The remainder in the exponent has a normal distribution, $Y_{t}-Y_{s}\sim\mathcal{N}(\mu(t-s),\sigma^{2}(t-s))$ . 

$$
{E \left[ X _ {t} | X _ {s}, s <   t \right]} = {e ^ {Y _ {s}} E \left[ e ^ {\mathcal {N} (\mu (t - s), \sigma^ {2} (t - s))} \bigg | Y _ {s}, s <   t \right]}
$$

Using the moment generating function for a normal distribution produces the result. 

$$
\begin{array}{r l r} {E \left[ X _ {t} | X _ {s}, s <   t \right]} & = & {e ^ {Y _ {s}} e ^ {\left(\mu + \frac {1}{2} \sigma^ {2}\right) (t - s)}} \\ & = & {X _ {s} e ^ {\left(\mu + \frac {1}{2} \sigma^ {2}\right) (t - s)}} \end{array}
$$

2. When would $e^{-rt}X_{t}$ be a martingale? 

(a) Relate the variables $r$ , $\mu$ , and $\sigma$ such that $e^{(-r + \mu + \frac{1}{2}\sigma^2)(t - s)} = 1$ (see below). 

(b) From part (a), $e^{-rt}$ is not random and can be removed from the expectation 

$$
\begin{array}{r c l} {E \left[ e ^ {- r t} X _ {t} \right| X _ {s}, s <   t ]} & = & {e ^ {- r t} X _ {s} e ^ {\left(\mu + \frac {1}{2} \sigma^ {2}\right) (t - s)}} \\ & = & {e ^ {- r s} e ^ {- r (t - s)} X _ {s} e ^ {\left(\mu + \frac {1}{2} \sigma^ {2}\right) (t - s)}} \end{array}
$$

For $e^{-rt}X_{t}$ to be a martingale, the right hand side must equal $e^{-rs}X_{s}$ . 

$$
\begin{array}{r c l} E \left[ e ^ {- r t} X _ {t} \mid X _ {s}, s <   t \right] & = & e ^ {- r s} X _ {s} \\ \Leftrightarrow e ^ {- r s} X _ {s} e ^ {- r (t - s)} e ^ {\left(\mu + \frac {1}{2} \sigma^ {2}\right) (t - s)} & = & e ^ {- r s} X _ {s} \\ \Leftrightarrow e ^ {- r (t - s)} e ^ {\left(\mu + \frac {1}{2} \sigma^ {2}\right) (t - s)} & = & 1 \\ \Leftrightarrow e ^ {\left(- r + \mu + \frac {1}{2} \sigma^ {2}\right) (t - s)} & = & 1 \\ \Leftrightarrow - r + \mu + \frac {1}{2} \sigma^ {2} & = & 0 \end{array}
$$

The above condition is satisfied when $\mu = r - \frac{1}{2}\sigma^2$ . Therefore, only choice (d) is suitable. 

3. $Z_{t} = e^{-rt}X_{t}$ where $X_{t} = e^{W_{t}}$ . This implies that $Z_{t} = e^{-rt + W_{t}}$ . 

(a) Expected value of increment $dZ_{t}$ is calculated using Ito's lemma. 

$$
\begin{array}{r c l} \frac {\partial Z _ {t}}{\partial t} & = & - r Z _ {t} \\ \frac {\partial Z _ {t}}{\partial W _ {t}} & = & \frac {\partial^ {2} Z _ {t}}{\partial^ {2} W _ {t}} = Z _ {t} \\ \Rightarrow d Z _ {t} & = & \left(\frac {1}{2} - r\right) Z _ {t} d t + Z _ {t} d W _ {t} \end{array}
$$

The expected value of the increment $dZ_{t}$ is $\left(\frac{1}{2} - r\right)Z_{t}dt$ . 

(b) Since the expected value of the increment is not zero, $Z_{t}$ cannot be a martingale (assuming $r \neq \frac{1}{2}$ ). 

(c) Calculate $E[Z_t]$ using $W_{t} \sim \mathcal{N}(0, t) \Rightarrow E[e^{W_t}] = e^{\frac{t}{2}}$ . 

$$
\begin{array}{r l r} {E [ Z _ {t} ]} & = & {e ^ {- r t} E [ e ^ {W _ {t}} ]} \\ & = & {e ^ {\left(- r + \frac {1}{2}\right) t}} \end{array}
$$

If the value $r$ is set to equal $\frac{1}{2}$ , then $Z_{t}$ is a martingale. From part (a), if $r = \frac{1}{2}$ , then $dZ_{t} = Z_{t}dW_{t}$ . This implies that $Z_{t}$ is a martingale. 

The exponential, $e^{X_t - \frac{1}{2}\langle X\rangle_t}$ , is a martingales if $X_{t}$ is a continuous martingale (with $X_0 = 0$ and for bounded $\langle X\rangle_t$ ). Therefore, inserting $\sqrt{2r}$ in front of the $W_{t}$ implies that $X_{t} = e^{\sqrt{2r}W_{t}}$ . Thus, $Z_{t} = e^{-rt + \sqrt{2r}W_{t}}$ is a martingale as $\left\langle \sqrt{2r}W_s\right\rangle_t = 2rt$ . 

(d) $Z_{t}$ is a mean one martingale, $E[Z_{t}|I_{0}] = Z_{0} = 1$ . 

## CHAPTER 14

1. (a) mean and variance of $\Delta X$ 

$$
\begin{array}{r l r} {E (\Delta X)} & = & {0. 3} \\ {V a r (\Delta X)} & = & {0. 1 9} \end{array}
$$

(b) If $\Delta Y = \Delta X - 0.25$ , then 

$$
E (\Delta Y) = 0. 0 5
$$

(c) No, the variance has not changed. 

(d) Choose 

$$
p = \left( \begin{array}{l} 0. 0 9 1 7 \\ 0. 3 1 9 0 \\ 0. 5 8 9 3 \end{array} \right)
$$

This results in 

$$
\begin{array}{r} E ^ {p} (\Delta X) = 0. 0 5 \\ V a r ^ {p} (\Delta X) = 0. 1 9 \end{array}
$$

The values for $p$ are chosen such that the elements of $p$ sum to 1 and $\Delta X$ maintains the same mean and variance. The following system of equations must be solved. 

$$
\left( \begin{array}{c c c} 1 & -. 5 & . 2 \\ (1 -. 0 5) ^ {2} & (-. 5 -. 0 5) ^ {2} & (. 2 -. 0 5) ^ {2} \\ 1 & 1 & 1 \end{array} \right) \left( \begin{array}{c} p _ {1} \\ p _ {2} \\ p _ {3} \end{array} \right) = \left( \begin{array}{c}. 0 5 \\ . 1 9 + (. 0 5) ^ {2} \\ 1 \end{array} \right)
$$

(e) The values of $\Delta X$ have not changed. Only the probabilities associated with the three values that $\Delta X$ can assume have changed. Thus, the distribution of $\Delta X$ has changed but not the state space of the random variable; $\Delta X$ remains an element of $\{1, -.5, .2\}$ . 

2. The density function $f(x)$ for $\log (R_t)$ is normal with mean $\mu$ and variance $\sigma^2$ . 

$$
f (x) = \frac {1}{\sqrt {2 \pi \sigma^ {2}}} e x p \left\{\frac {- (x - \mu) ^ {2}}{2 \sigma^ {2}} \right\}
$$

(a) Choose 

$$
\xi (x) = \exp \left\{\frac {1}{2 \sigma^ {2}} \left[ - (x - r) ^ {2} + (x - \mu) ^ {2} \right] \right\},
$$

The density $\xi (x)f(x)$ is a normal density with mean $r$ and variance $\sigma^2$ . 

(b) Choose 

$$
\xi (x) = \exp \left\{\frac {1}{2 \sigma^ {2}} \left[ - x ^ {2} + (x - \mu) ^ {2} \right] \right\},
$$

and the density $\xi (x)f(x)$ is a normal density with mean 0 and variance $\sigma^2$ . 

(c) It is easier to calculate $E(R_t^2)$ under the distribution in (b) since $E(R_t^2) = Var(R_t) = \sigma^2$ because the distribution in part (b) has mean zero. 

(d) No, the variance has not changed. Both transformations adjusted the mean but not the variance. 

3. (a) Plot of the joint density: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5882bd1f-b733-4ed9-8bdc-4c98ae290af0/cf5a5effc3bc1643e64ff934921156f79408114f18ec33599c9fee42b3e835e6.jpg)



FIGURE 0.14 Plot of bivariate normal density function with mean $\mu$ and var-cov $\Sigma$ .


(b) Choose 

$$
\xi (x) = \exp \left\{- \frac {1}{2} \left[ x ^ {\prime} \Sigma^ {- 1} x - (x - \mu) ^ {\prime} \Sigma^ {- 1} (x - \mu) \right] \right\},
$$

where $x$ is a 2 - vector. The density $\xi([R, r])f(R, r)$ is multivariate normal with mean 0 and variance-covariance matrix $\Sigma$ . 

(c) Plot of the new joint density: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5882bd1f-b733-4ed9-8bdc-4c98ae290af0/f178420c3b091fc54d6ab9f8792b52cee6446ab6c15192093206b46a795dd8bd.jpg)



FIGURE 0.15 Plot of bivariate normal density function with 0 mean and var-cov $\Sigma$



(d) No, the variance - covariance matrix has not changed.


## CHAPTER 15

1. (a) 

$$
\begin{array}{r c l} C (t, S _ {t}) - P (t, S _ {t}) & = & e ^ {- r (T - t)} E (\max (S _ {T} - K, 0) | \mathcal {I} _ {t}) - e ^ {- r (T - t)} E (\max (K - S _ {T}, 0) | \mathcal {I} _ {t}) \\ & = & e ^ {- r (T - t)} E (\max (S _ {T} - K, 0) - \max (K - S _ {T}, 0) | \mathcal {I} _ {t}) \\ & = & e ^ {- r (T - t)} E (\max (S _ {T} - K, 0) + \min (S _ {T} - K, 0) | \mathcal {I} _ {t}) \\ & = & e ^ {- r (T - t)} E (S _ {T} - K | \mathcal {I} _ {t}) \\ & = & S _ {t} - e ^ {- r (T - t)} K \end{array}
$$

since under the risk - neutral measure, the discounted stock is a martingale. This relationship is put - call parity. 

(b) This follows trivially by part (a) and the definition of $H(t, S_t)$ . 

(c) By part (b) 

$$
\begin{array}{r c l} {H (t, S _ {t})} & = & {\max \left[ C (t, S _ {t}), C (t, S _ {t}) + e ^ {- r (T - t)} K - S _ {t} \right]} \\ & = & {C (t, S _ {t}) + \max \left[ e ^ {- r (T - t)} K - S _ {t}, 0 \right]} \end{array}
$$

Therefore 

$$
\begin{array}{r c l} H (0, S _ {0}) & = & e ^ {- r t} E \left(C (t, S _ {t}) + \max \left[ e ^ {- r (T - t)} K - S _ {t}, 0 \right]\right) \\ & = & e ^ {- r t} C (0, S) e ^ {r t} + e ^ {- r t} E \left(\max \left[ e ^ {- r (T - t)} K - S _ {t}, 0 \right]\right) \\ & = & C (0, S _ {0}) + e ^ {- r t} e ^ {- r (T - t)} E \left(\max \left[ K - e ^ {r (T - t)} S _ {t}, 0 \right]\right) \\ & = & C (0, S _ {0}) + e ^ {- r T} E \left(\max \left[ K - e ^ {r (T - t)} S _ {t}, 0 \right]\right) \end{array}
$$

With $S_{t} = S_{0}e^{(r - \frac{1}{2}\sigma^{2})t + \sigma W_{t}}$ under the risk-neutral measure, the result follows. 

(d) Since $e^{-rT}E\left(\max\left[K-e^{r(T-t)}S_{t},0\right]\right)=e^{-r(T-t)}E\left(\max\left[e^{-r(T-t)}K-S_{t},0\right]\right)$ , the chooser option is equivalent to a portfolio consisting of a long call expiring at T with strike K plus a long put with strike $Ke^{-r(T-t)}$ expiring at t. Therefore 

$$
H (0, S _ {0}) = C (0, S _ {0}, K, T) + P (0, S _ {0}, K e ^ {- r (T - t)}, t)
$$

(e) Using the Black-Scholes formula 

$$
H (0, S _ {0}) = S _ {0} (N (d _ {1}) - N (- \overline {{d}} _ {1})) + K e ^ {- r (t - T)} (N (- \overline {{d}} _ {2}) - N (d _ {2}))
$$

where 

$$
\begin{array}{r l r} {d _ {1}} & = & {\frac {\ln \left(\frac {S _ {0}}{K}\right) + \left(r + \frac {1}{2} \sigma^ {2}\right) T}{\sigma \sqrt {T}}} \\ {d _ {2}} & = & {d _ {1} - \sigma \sqrt {T}} \end{array}
$$

and 

$$
\begin{array}{r l r} {\overline {{d}} _ {1}} & = & {\frac {\ln \left(\frac {S _ {0}}{K}\right) + r T + \frac {1}{2} \sigma^ {2} t}{\sigma \sqrt {t}}} \\ {\overline {{d}} _ {2}} & = & {\overline {{d}} _ {1} - \sigma \sqrt {t}} \end{array}
$$

2. (a) Use Ito's lemma to show that 

$$
S _ {t} = S _ {0} e ^ {(r - f - \frac {1}{2} \sigma^ {2}) t + \sigma W _ {t}}
$$

is the solution to the SDE 

$$
d S _ {t} = (r - f) S _ {t} d t + \sigma S _ {t} d W _ {t}
$$

Taking $S_{t} = f(t,W_{t}) = S_{0}e^{(r - f - \frac{1}{2}\sigma^{2})t + \sigma W_{t}}$ and applying Ito's lemma 

$$
\begin{array}{r c l} {d S _ {t}} & = & {\frac {\partial f}{\partial t} d t + \frac {\partial f}{\partial W _ {t}} d W _ {t} + \frac {1}{2} \frac {\partial^ {2} f}{\partial^ {2} W _ {t}} d t} \\ & = & {\left(r - f - \frac {1}{2} \sigma^ {2}\right) S _ {t} d t + \sigma S _ {t} d W _ {t} + \frac {1}{2} \sigma^ {2} S _ {t} d t} \\ & = & {\left[ r - f - \frac {1}{2} \sigma^ {2} + \frac {1}{2} \sigma^ {2} \right] S _ {t} d t + \sigma S _ {t} d W _ {t}} \\ & = & {(r - f) S _ {t} d t + \sigma S _ {t} d W _ {t}} \end{array}
$$

(b) For s > 0 consider the conditional expectation 

$$
\begin{array}{r c l} E \left[ e ^ {\sigma W _ {t + s} - \frac {1}{2} \sigma^ {2} (t + s)} \right| \mathcal {I} _ {t} & = & e ^ {- \frac {1}{2} \sigma^ {2} (t + s) + \sigma W _ {t}} E \left[ e ^ {\sigma \Delta W _ {t}} \right] \\ & = & e ^ {- \frac {1}{2} \sigma^ {2} (t + s) + \sigma W _ {t} + \frac {1}{2} \sigma^ {2} s} \\ & = & e ^ {- \frac {1}{2} \sigma^ {2} t + \sigma W _ {t}} \end{array}
$$

Thus, the process is a martingale. The second equality follows from $\Delta W_{t} = W_{t + s} - W_{t}\sim \mathcal{N}(0,s)$ . Therefore, $E\left[e^{\sigma (W_{t + s} - W_t)}\right] = e^{\frac{1}{2}\sigma^2 s}$ by the moment generating function for the normal distribution. 

(c) If $X_{u} = \sigma$ , then by Girsanov's theorem 

$$
\begin{array}{r c l} \tilde {W} _ {t} & = & W _ {t} - \int_ {0} ^ {t} X _ {u} d u \\ & = & W _ {t} - \sigma t \end{array}
$$

is a martingale under the measure $\tilde{P}$ where 

$$
\tilde {P} (A) = \int_ {A} \xi (W _ {T}) d P
$$

and 

$$
\begin{array}{r l r} \xi (W _ {T}) & = & e ^ {\int_ {0} ^ {T} X _ {u} d W _ {u} - \frac {1}{2} \int_ {0} ^ {T} X _ {u} ^ {2} d u} \\ & = & e ^ {\sigma W _ {T} - \frac {1}{2} \sigma^ {2} T} \end{array}
$$

(d) Let $Z_{t} = f(S_{t}) = \frac{1}{S_{t}} = \frac{1}{S_{0}} e^{-(r - f - \frac{1}{2}\sigma^{2})t - \sigma W_{t}}$ . By Ito's lemma 

$$
\begin{array}{r c l} {d Z _ {t}} & = & {\frac {\partial f}{\partial t} d t + \frac {\partial f}{\partial W _ {t}} d W _ {t} + \frac {1}{2} \frac {\partial^ {2} f}{\partial^ {2} W _ {t}} d t} \\ & = & {\frac {- (r - f - \frac {1}{2} \sigma^ {2})}{S _ {t}} d t - \frac {\sigma}{S _ {t}} d W _ {t} + \frac {1}{2} \frac {\sigma^ {2}}{S _ {t}} d t} \\ & = & {\frac {1}{S _ {t}} [ f - r + \frac {1}{2} \sigma^ {2} + \frac {1}{2} \sigma^ {2} ] d t - \frac {1}{S _ {t}} \sigma d W _ {t}} \\ & = & {Z _ {t} [ f - r + \sigma^ {2} ] d t - Z _ {t} \sigma d W _ {t}} \end{array}
$$

(e) For $s > 0$ , consider the conditional expectation under measure $P$ and define $\Delta W_{t} = W_{t + s} - W_{t}$ . 

$$
\begin{array}{r l r} {E \left[ Z _ {t + s} | \mathcal {I} _ {t} \right]} & = & {\frac {1}{S _ {0}} e ^ {- (r - f - \frac {1}{2} \sigma^ {2}) (t + s) - \sigma W _ {t}} E \left[ e ^ {- \sigma \Delta W _ {t}} \right]} \\ & = & {\frac {1}{S _ {0}} e ^ {- (r - f - \frac {1}{2} \sigma^ {2}) (t + s) - \sigma W _ {t}} e ^ {\frac {1}{2} \sigma^ {2} s}} \end{array}
$$

Therefore 

$$
\begin{array}{r c l} E \left[ \frac {Z _ {t + s} e ^ {r (t + s)}}{e ^ {f (t + s)}} \middle | \mathcal {I} _ {t} \right] & = & \frac {1}{S _ {0}} e ^ {- (r - f - \frac {1}{2} \sigma^ {2}) (t + s) - \sigma W _ {t} + \frac {1}{2} \sigma^ {2} s + (r - f) (t + s)} \\ & = & \frac {1}{S _ {0}} e ^ {\frac {1}{2} \sigma^ {2} (t + s) - \sigma W _ {t} + \frac {1}{2} \sigma^ {2} s} \\ & \neq & \frac {1}{S _ {0}} e ^ {\frac {1}{2} \sigma^ {2} t - \sigma W _ {t}} \\ & = & Z _ {t} e ^ {(r - f) t} \end{array}
$$

and the process is not a martingale under measure P. However, under measure $\tilde{P}$ , the situation changes. The term $\Delta W_{t}$ under measure P is $\mathcal{N}(0,s)$ while under measure $\tilde{P}$ , the variance remains the same but the mean changes according to part (c). Under measure $\tilde{P}$ , use the property that $W_{t}=\tilde{W}_{t}+\sigma t$ to conclude that 

$$
\begin{array}{r c l} \Delta W _ {t} & = & W _ {t + s} - W _ {t} \\ & = & \tilde {W} _ {t + s} + \sigma (t + s) - (\tilde {W} _ {t} + \sigma t) \\ & = & \tilde {W} _ {t + s} - \tilde {W} _ {t} + \sigma s \\ & = & \Delta \tilde {W} _ {t} + \sigma s \end{array}
$$

Since $\Delta \tilde{W}_t\stackrel {d}{\sim}\mathcal{N}(0,s)$ under measure $\tilde{P}$ 

$$
\begin{array}{r c l} E ^ {\tilde {P}} \left[ e ^ {- \sigma \Delta W _ {t}} \right] & = & E ^ {\tilde {P}} \left[ e ^ {- \sigma (\sigma s + \Delta \tilde {W} _ {t})} \right] \\ & = & E ^ {\tilde {P}} \left[ e ^ {- \sigma^ {2} s - \sigma \Delta \tilde {W} _ {t}} \right] \\ & = & E ^ {\tilde {P}} \left[ e ^ {- \sigma^ {2} s + \mathcal {N} (0, \sigma^ {2} s)} \right] \\ & = & e ^ {- \sigma^ {2} s} E ^ {\tilde {P}} \left[ e ^ {\mathcal {N} (0, \sigma^ {2} s)} \right] \\ & = & e ^ {- \sigma^ {2} s + \frac {1}{2} \sigma^ {2} s} \end{array}
$$

This result is used below. 

$$
\begin{array}{r c l} E ^ {\tilde {P}} \left[ Z _ {t + s} | \mathcal {I} _ {t} \right] & = & \frac {1}{S _ {0}} e ^ {- (r - f - \frac {1}{2} \sigma^ {2}) (t + s) - \sigma W _ {t}} E ^ {\tilde {P}} \left[ e ^ {- \sigma \Delta W _ {t}} \right] \\ & = & \frac {1}{S _ {0}} e ^ {- (r - f - \frac {1}{2} \sigma^ {2}) (t + s) - \sigma W _ {t} - \sigma^ {2} s + \frac {1}{2} \sigma^ {2} s} \\ & = & \frac {1}{S _ {0}} e ^ {- (r - f) (t + s) + \frac {1}{2} \sigma^ {2} t - \sigma W _ {t}} \end{array}
$$

Therefore 

$$
\begin{array}{r l r} {E ^ {\tilde {P}} \left[ \frac {Z _ {t + s} e ^ {r (t + s)}}{e ^ {f (t + s)}} \bigg | \mathcal {I} _ {t} \right]} & = & {\frac {1}{S _ {0}} e ^ {\frac {1}{2} \sigma^ {2} t - \sigma W _ {t}}} \\ & = & {Z _ {t} \frac {e ^ {r t}}{e ^ {f t}}} \end{array}
$$

and the process is a martingale under $\tilde{P}$ . 

(f) Yes, $Z_{t}$ is the price of 1 unit of domestic currency in terms of foreign currency. In order to discount this quantity, multiply by $\frac{e^{rt}}{e^{ft}} = e^{(r - f)t}$ . Thus, $\tilde{P}$ is the arbitrage-free measure of the foreign economy. 

## CHAPTER 16

## 1. Payoff Diagrams

(a) A caplet with rate $R_{cap} = 6.75\%$ written on 3 - month Libor. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5882bd1f-b733-4ed9-8bdc-4c98ae290af0/8628efbf4e6082bf3f27041784da6e624ba60276457f787065ed29e236faa6c0.jpg)



Payoff of a Single FRA on 3-month Libor with F equal to 7.5%


(b) A forward contract maturing in 3 months on a default - free discount bond whose maturity is 18 months. The contracted price is 89.5. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5882bd1f-b733-4ed9-8bdc-4c98ae290af0/8eb68b3d1aa6f8bb32c14ae22597c686e223380147a07228103e9fb5f78daf99.jpg)



(c) A 3 by 6 FRA that pays a 3 - month fixed rate, $F = 7.5\%$ , against Libor.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5882bd1f-b733-4ed9-8bdc-4c98ae290af0/fa477f2464243f761398ad0a10c449b1c91e4a3e44e78e046a390dfe2f5e5bf3.jpg)


(d) A fixed payer interest rate swap with swap rate $\kappa = 7.5\%$ which receives 6 - month Libor. The swap began 6 months ago and matures in 2 years. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5882bd1f-b733-4ed9-8bdc-4c98ae290af0/9d37ee5f2db6416d83b944b08e8ba73f1ee34a9405428114eb94b4f6ff16faac.jpg)



(e) A swaption maturing in 6 months on a 2 year fixed paper swap with swap rate $\kappa = 6\%$ .


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5882bd1f-b733-4ed9-8bdc-4c98ae290af0/8b793dc90d46dbeaa51bdfef18052020540d46979184331f404ca1bd7c6d39a4.jpg)



2. The assets which trade are (b), (c), (d), and (g). Returns and volatilities do not trade and must be inferred from assets such as bonds or options.


## CHAPTER 17

1. Construct an implied tree for the spot rate process $dr_{t} = .01r_{t}dt + .12r_{t}dW_{t}$ 

(a) Choose $\Delta$ to have 5 time steps in a 12 month period; $\Delta = \frac{12}{5}$ months or $\frac{1}{5}$ years. 

(b) Since $\Delta$ and $\sigma$ are fixed constants, $u = e^{\sigma \sqrt{\Delta}} = e^{(.12)\sqrt{\frac{1}{5}}} = 1.0551$ and $d = \frac{1}{u} = .9477$ are also constant throughout the tree. 

(c) The tree is recombining with $t + 1$ nodes at time t. 

$$
\begin{array}{c c c c c c} t = 0 & t = 1 & t = 2 & t = 3 & t = 4 & t = 5 \\ \hline & & & & & 0. 0 7 8 5 \\ & & & & 0. 0 7 4 4 \\ & & & 0. 0 7 0 5 & & 0. 0 7 0 5 \\ & & 0. 0 6 6 8 & & 0. 0 6 6 8 \\ & 0. 0 6 3 3 & & 0. 0 6 3 3 & & 0. 0 6 3 3 \\ 0. 0 6 0 0 & & 0. 0 6 0 0 & & 0. 0 6 0 0 \\ & 0. 0 5 6 9 & & 0. 0 5 6 9 & & 0. 0 5 6 9 \\ & & 0. 0 5 3 9 & & 0. 0 5 3 9 \\ & & & 0. 0 5 1 1 & & 0. 0 5 1 1 \\ & & & & 0. 0 4 8 4 \\ & & & & & 0. 0 4 5 9 \end{array}
$$

(d) As no traded bonds have been introduced into the economy, it is not possible to find the term structure market price of risk. Nor can risk - neutral probabilities be ascertained. However, empirical probabilities can be obtained using the original SDE. Consider the discretized SDE with partition size $\Delta$ under the empirical measure 

$$
r _ {t + 1} = r _ {t} + \mu \Delta r _ {t} + \sigma r _ {t} \Delta W
$$

Given this process, the following reasoning extracts probabilities from the spot rate tree. 

$$
E [ r _ {t + 1} ] = r _ {t} + \mu \Delta r _ {t}
$$

$$
\begin{array}{r l} \Rightarrow & p ^ {u} (t) r _ {t + 1} ^ {u} + (1 - p ^ {u} (t)) r _ {t + 1} ^ {d} = r _ {t} + \mu \Delta r _ {t} \\ \Rightarrow & p ^ {u} (t) (r _ {t + 1} ^ {u} - r _ {t + 1} ^ {d}) = r _ {t} + \mu \Delta r _ {t} - r _ {t + 1} ^ {d} \end{array}
$$

Therefore, $p^u(t) = \frac{r_t + \mu\Delta r_t - r_{t + 1}^d}{r_{t + 1}^u - r_{t + 1}^d}$ 

The “up” probabilities: 

$$
\begin{array}{c c c c c} t = 0 & t = 1 & t = 2 & t = 3 & t = 4 \\ & & & & 0. 5 0 6 1 \\ & & & 0. 5 3 1 8 \\ & & 0. 5 0 4 7 & & 0. 5 0 4 7 \\ & 0. 5 0 3 9 & & 0. 5 0 3 9 \\ 0. 5 0 3 1 & & 0. 5 0 3 1 & & 0. 5 0 3 1 \\ & 0. 5 1 0 5 & & 0. 5 1 0 5 \\ & & 0. 5 0 1 3 & & 0. 5 0 1 3 \\ & & & 0. 5 0 9 5 \\ & & & & 0. 4 9 9 4 \end{array}
$$

The “down” probabilities: 

$$
\begin{array}{c c c c c} t = 0 & t = 1 & t = 2 & t = 3 & t = 4 \\ \hline & & & & 0. 4 9 3 9 \\ & & & 0. 4 6 8 2 \\ & & 0. 4 9 5 3 & & 0. 4 9 5 3 \\ 0. 4 9 6 9 & 0. 4 9 6 1 & 0. 4 9 6 9 & 0. 4 9 6 1 \\ & 0. 4 8 9 5 & 0. 4 9 6 9 & & 0. 4 9 6 9 \\ & & 0. 4 8 9 5 & 0. 4 8 9 5 \\ & & 0. 4 9 8 7 & & 0. 4 9 8 7 \\ & & & 0. 4 9 0 5 \\ & & & & 0. 5 0 0 6 \end{array}
$$

2. Given 4 zero coupon bonds of different maturities, construct a “tree” for the spot rate which is consistent with the observed bond prices. 

(a) There are at least two methods to generate a “tree”. The second generates a spot rate tree for a specified volatility term structure given by the Black, Derman, and Toy model. The first method simply finds the implied forward curve from market observed bond prices. These implied forward rates are not necessarily expected future spot rates. However, they are very useful objects in the study of fixed income securities. 

## (b) Method 1 - Forward Rate Curve

Implied forward rates can be ascertained from default - free zero coupon bonds recursively. This procedure starts with the shortest maturity bond and finds an implied spot rate assumed to be constant from period 0 until 1. Then, the procedure uses the two year bond to find an implied rate between 1 and 2. Repeating the procedure with consecutively longer maturities extrapolates a piecewise constant approximation to the forward rate curve. 

Want to find forward rates between time $t_{i-1}$ and $t_i$ . 

$$
\frac {1}{1 + f _ {0 , 1}} = . 9 4 \Rightarrow f _ {0, 1} = \frac {1}{. 9 4} - 1 = . 0 6 3 8 3
$$

$$
\left(\frac {1}{1 + f _ {0 , 1}}\right) \left(\frac {1}{1 + f _ {1 , 2}}\right) = . 9 2 \Rightarrow f _ {1, 2} = \frac {1}{. 9 2 (1 + f _ {0 , 1})} - 1 = . 0 2 1 7 4
$$

The other two rates are obtained in a similar fashion. 

$$
\begin{array}{r c l} f _ {2, 3} & = & \frac {1}{. 8 7 (1 + f _ {0 , 1}) (1 + f _ {1 , 2})} - 1 = . 0 5 7 4 8 \\ f _ {3, 4} & = & \frac {1}{. 8 0 (1 + f _ {0 , 1}) (1 + f _ {1 , 2}) (1 + f _ {2 , 3})} - 1 = . 0 8 7 4 9 \end{array}
$$

Method 2 - Assume a Volatility Term Structure and Implement Black Derman and Toy (BDT) Model 

The (BDT) model requires a term structure of yields and volatilities. Here, the volatility term structure is a flat .12 from the above equation. In addition, the yield at maturity $N$ , $y_{N}$ , is implied from bond prices by the formula $P(0,N) = \frac{1}{(1 + y_N)^N}$ . 

<table><tr><td>Maturity</td><td>Yield</td><td>Volatility</td></tr><tr><td>1</td><td>.06383</td><td>.12</td></tr><tr><td>2</td><td>.04257</td><td>.12</td></tr><tr><td>3</td><td>.04751</td><td>.12</td></tr><tr><td>4</td><td>.05737</td><td>.12</td></tr></table>

The first node of the tree is implied directly from $P(0,1)$ and is equal to .06383 while $r_u$ and $r_d$ require two equations to match yields and volatilities. The volatilities must satisfy $\sigma = .12 = \frac{\ln\left(\frac{r_u}{r_d}\right)}{2} \Rightarrow r_u = r_d e^{-24}$ . Therefore, there are two equations and two unknowns ( $r_u$ and $r_d$ ). 

$$
\begin{array}{r l} & {\frac {\frac {1}{2} \left[ \frac {1}{1 + r _ {u}} + \frac {1}{1 + r _ {d}} \right]}{1 . 0 6 3 8 3} = P (0, 2) = . 9 2} \\ & {(2) r _ {u} = r _ {d} e ^ {. 2 4}} \\ & {\Rightarrow \frac {1}{1 + r _ {d} e ^ {. 2 4}} + \frac {1}{1 + r _ {d}} = 2 (1. 0 6 3 8 3) (. 9 2)} \end{array}
$$

The values $r_{u} = .024342$ and $r_{d} = .019148$ are the solutions. As the forward rates indicate, there is a drop in interest rates between period 1 and 2. Next, solve for $r_{uu}$ , $r_{dd}$ , and $r_{ud} = r_{du}$ . These are related by $r_{uu} = e^{\cdot24}r_{ud} = e^{\cdot48}r_{dd}$ and satisfy the equation 

$$
\frac {\frac {1}{1 + r _ {d d} e ^ {. 4 8}} + \frac {1}{1 + r _ {u d} e ^ {. 2 4}}}{1 . 0 2 4 3 4 2} + \frac {\frac {1}{1 + r _ {u d} e ^ {. 2 4}} + \frac {1}{1 + r _ {d d}}}{1 . 0 1 9 1 4 8} = 4 (1. 0 6 3 8 3) (. 8 7)
$$

The values $r_{uu} = .072153$ , $r_{ud} = .056758$ , and $r_{dd} = .072153$ are the solutions. Thus far, the tree has become 

$$
\begin{array}{c c c} \text {t = 0} & \text {t = 1} & \text {t = 2} \\ & & 0. 0 7 2 1 5 3 \\ & 0. 0 2 4 3 4 2 \\ 0. 0 6 3 8 3 & & 0. 0 5 6 7 5 8 \\ & 0. 0 1 9 1 4 8 & \\ & & 0. 0 4 4 6 4 7 \end{array}
$$

The solutions for $r_{uuu}$ , $r_{ddd}$ , etc proceeds in a similar manner. 

(c) The difference between the methods in problem 1 and 2 involves the information contained in market observed bond prices. The two approaches taken in problem 2 are consistent with the market prices of bonds used for calibrating the term structure. However, errors between observed bond prices and bond prices implied by the term structure could occur in other additional bonds not used to infer the term structure. Problem 1 assumed a process for the spot rate but bond prices derived from the spot rate process need not match any observed bond prices. Thus, without placing additional restrictions on the parameters of the spot rate process in problem 1, the model may not be consistent with observed bond prices which could generate arbitrage opportunities. 

3. Process for the spot rate is $dr_{t} = .02r_{t}dt + .06r_{t}dW_{t}$ with $r_{0} = .06$ . 

(a) Discretize the SDE at nodes $t_0 = 0 < t_1 < t_2 < \ldots < t_n = t$ and define $\Delta = t_i - t_{i-1}$ . 

$$
r _ {t _ {i}} = r _ {t _ {i - 1}} +. 0 2 r _ {t _ {i - 1}} \Delta +. 0 6 r _ {t _ {i - 1}} \Delta W
$$

(b) see MATLAB program below 

(c) A MATLAB program to calculate the integral is below. 

```matlab
delta=.04
t=1;
%number of nodes (not including the first)
n=t/delta;
r=zeros(n,1);
%starting value is .06
r(1)=.06;

for k=1:1000

for i=2:n
    %generate random increment
    deltaW=normrnd(0,sqrt(delta));
    r(i) = r(i-1) + .02*r(i-1)*delta + .06*r(i-1)*deltaW;
end

%approximate integral with sum
%the partition width is fixed at .04 making the approximation .04 times the
%sum of all the entries

%calculate the first expectation in part (c)
expect1(k)=exp(-.04*sum(r));
%calculate the second expectation in part (c)
expect2(k)=max(r(n)-.06,0);
%calculate the expectation in part (b) (combined expectations)
expect3(k)=exp(-.04*sum(r)) * max(r(n)-.06,0);

end

%calculate final values for comparison
E1=mean(expect1);
E2=mean(expect2); 
```

```matlab
E3=mean(expect3);
difference = E3-E1*E2
-2.2972e-06 
```

(d) In general, unless the random variables $X$ and $Y$ are uncorrelated, one cannot separate $E[XY]$ into $E[X]E[Y]$ . For instance, if $\max (r_1 - .06, 0)$ is large, then the value of $r_1$ must have been large. However, this would imply a smaller value for $e^{-\int_0^1 r_s ds}$ . 

$$
E \left[ e ^ {- \int_ {0} ^ {1} r _ {s} d s} \max (r _ {1} -. 0 6, 0) \right] \neq E \left[ e ^ {- \int_ {0} ^ {1} r _ {s} d s} \right] E \left[ \max (r _ {1} -. 0 6, 0) \right]
$$

The quantity difference in the output of the above program, although small in this example, provides empirical justification for not separating the expectations. 

(e) Bond prices are calculated under the equivalent risk - neutral martingale measure when using spot rate data, not the empirical measure. 

$$
P (t, T) = E _ {t} ^ {\tilde {P}} \left[ e ^ {- \int_ {t} ^ {T} r (s) d s} \right]
$$

The market price of risk is required to calculate the expectation under the correct measure. 

(f) The interest rate dynamics would be arbitrage - free if, using the formula above, they generated bond prices which matched those observed in the market. One requires a traded asset such as a bond in order to make any conclusions regarding arbitrage opportunities. 

(g) If the spot rate process is changed to a equivalent risk - neutral martingale measure, a market price of risk, $\lambda_{t}$ , would be introduced into the drift of the process. This market price of risk is the compensation investors require when faced with uncertainty in the spot rate caused by the Brownian motion. The spot rate process under the risk - neutral measure would be 

$$
d r _ {t} = (. 0 2 +. 0 6 \lambda_ {t}) r _ {t} d t +. 0 6 r _ {t} d \tilde {W} _ {t}
$$

where $\tilde{W}_t$ is a Brownian motion under the equivalent risk-neutral martingale measure, $\tilde{P}$ . 

(h) A set of arbitrage - free bonds could determine the unknown market price of risk as in the Heath, Jarrow, and Morton term structure model. 

## CHAPTER 18

1. Consider the Vasicek spot rate model, $dr_{t} = \alpha(\mu - r_{t})dt + \sigma dW_{t}$ , which incorporates mean reversion into the spot rate. The term $\mu$ represents the long term average spot rate while $\alpha$ represents the “speed” of reversion from $r_{t}$ to $\mu$ . Both quantities $\alpha$ and $\mu$ are positive. 

(a) Solve for $E[r_s|r_t]$ and $Var[r_s|r_t]$ for $t < s$ . 

$\begin{array}{rcl}d r_t & = & \alpha (\mu -r_t)dt + \sigma dW_t\\ dr_t + \alpha r_t dt & = & \alpha \mu dt + \sigma dW_t\quad \mathrm{m u l t i p l y b o t h s i d e s b y}e^{\alpha t}\\ e^{\alpha t}[dr_t + \alpha r_t dt] & = & e^{\alpha t}[\alpha \mu dt + \sigma dW_t]\\ \frac{\partial}{\partial t}\left[e^{\alpha t}r_t\right] & = & e^{\alpha t}[\alpha \mu dt + \sigma dW_t]\quad \mathrm{integrate from}t\mathrm{to}s\\ \int_t^s\frac{\partial}{\partial x}\left[e^{\alpha x}r_x\right]dx & = & \alpha \mu \int_t^s e^{\alpha x}dx + \sigma \int_t^s e^{\alpha x}dW_x\\ e^{\alpha x}r_x|_{x = t}^{x = s} & = & \mu e^{\alpha x}|_{x = t}^{x = s} + \sigma \int_t^s e^{\alpha x}dW_x\\ e^{\alpha s}r_s - e^{\alpha t}r_t & = & \mu e^{\alpha s} - \mu e^{\alpha t} + \sigma \int_t^s e^{\alpha x}dW_x\quad \mathrm{m u l t i p l y by}e^{-\alpha s}\\ r_s & = & e^{-\alpha (s - t)}r_t + \mu -\mu e^{-\alpha (s - t)} + \sigma e^{-\alpha s}\int_t^s e^{\alpha x}dW_x\\ r_s & = & \mu +(r_t - \mu)e^{-\alpha (s - t)} + \sigma e^{-\alpha s}\int_t^s e^{\alpha x}dW_x \end{array}$ 

From the above equation, the conditional mean and variance are obtained. 

$$
\begin{array}{r c l} {E \left[ r _ {s} | r _ {t} \right]} & = & {\mu + (r _ {t} - \mu) e ^ {- \alpha (s - t)} \qquad \mathrm{since} E \left[ \sigma e ^ {- \alpha s} \int_ {t} ^ {s} e ^ {\alpha x} d W _ {x} \right] = 0} \\ {V a r \left[ r _ {s} | r _ {t} \right]} & = & {V a r \left[ \sigma e ^ {- \alpha s} \int_ {t} ^ {s} e ^ {\alpha x} d W _ {x} \right]} \\ & = & {\sigma^ {2} e ^ {- 2 \alpha s} \left\langle \int_ {t} ^ {\cdot} e ^ {\alpha x} d W _ {x} \right\rangle_ {s}} \end{array}
$$

$$
\begin{array}{r l} {=} & {\sigma^ {2} e ^ {- 2 \alpha s} \int_ {t} ^ {s} e ^ {2 \alpha x} d x} \\ {=} & {\frac {\sigma^ {2}}{2 \alpha} \left[ 1 - e ^ {- 2 \alpha (s - t)} \right]} \end{array}
$$

The second equality in the variance calculation is the Ito isometry 

$$
V a r \left(\int_ {0} ^ {t} f (u) d W _ {u}\right) = \left\langle \int_ {0} ^ {\cdot} f (u) d W _ {u} \right\rangle_ {t} = \int_ {0} ^ {t} f ^ {2} (u) d u
$$

provided that the integrand $f(\cdot)$ is predictable. 

(b) As $s \uparrow \infty$ for a fixed $t$ , the terms $e^{-\alpha s}$ and $e^{-\alpha (s - t)}$ converge to zero since $\alpha$ is a positive constant. Therefore, the conditional mean approaches $\mu$ and the conditional variance approaches $\frac{\sigma^2}{2\alpha}$ . 

(c) Calculate the coefficients for the bond dynamics. This requires $B_{r}(t,s)$ , the partial derivative of the bond maturing at time s with respect to spot interest rate at time t, $r(t)$ . Using the formula found in the text, $\mu^{B}B = r_{t}B + \sigma B_{r}\lambda$ , results in the drift coefficient $\mu^{B}$ being isolated. To calculate $B_{r}$ , substitute $r(s)$ above into the bond price with v replacing s and adjust spot rate dynamics to account for the market price of risk. 

$$
\begin{array}{r c l} B (t, s) & = & E _ {t} ^ {\tilde {P}} \left[ e ^ {- \int_ {t} ^ {s} r _ {v} d v} \right] \\ & = & E _ {t} \left[ e ^ {- \int_ {t} ^ {s} (\mu + (r _ {t} - \mu) e ^ {- \alpha (v - t)} + \sigma e ^ {- \alpha v} \int_ {t} ^ {v} e ^ {\alpha x} (d \tilde {W} _ {x} + \lambda d x)) d v} \right] \\ & = & E _ {t} \left[ e ^ {- r _ {t} \int_ {t} ^ {s} e ^ {- \alpha (v - t)} d v} e ^ {- \int_ {t} ^ {s} (\mu - \mu e ^ {- \alpha (v - t)} + \sigma e ^ {- \alpha v} \int_ {t} ^ {v} e ^ {\alpha x} (d \tilde {W} _ {x} + \lambda d x)) d v} \right] \\ \Rightarrow B _ {r} = \frac {\partial B (t , s)}{\partial r (t)} & = & - \left(\int_ {t} ^ {s} e ^ {- \alpha (v - t)} d v\right) B (t, s) \\ & = & \frac {(e ^ {- \alpha (s - t)} - 1)}{\alpha} B (t, s) \end{array}
$$

Therefore 

$$
{B _ {r}} = {- B \frac {(1 - e ^ {- \alpha (s - t)})}{\alpha} <   0}
$$

With $\alpha > 0$ and s - t > 0, $B_{r}$ is negative since $e^{-\alpha(s-t)} - 1 < 0$ . The sign of this partial derivative is intuitive as an increase in the spot interest rate lowers bond prices. The drift of the bond equals 

$$
\begin{array}{r c l} \mu^ {B} B & = & r _ {t} B + \sigma B _ {r} \lambda \\ \mu^ {B} & = & r _ {t} + \frac {\sigma \lambda}{\alpha} \left(1 - e ^ {- \alpha (s - t)}\right) > r _ {t} \end{array}
$$

Here, a slight adjustment was made to ensure that $\mu^{B}$ is greater than $r_{t}$ . To solve for $\sigma^{B}$ , the relationship $\sigma^{B}B = b(r_{t}, t)B_{r}$ is used where in this instance $b(r_{t}, t) = \sigma$ . The negative sign is removed as the standard deviation must be positive. 

$$
\begin{array}{r c l} \sigma^ {B} B & = & b (r _ {t}, t) B _ {r} \\ \sigma^ {B} & = & \frac {\sigma}{\alpha} \left(1 - e ^ {- \alpha (s - t)}\right) > 0 \end{array}
$$

The values of $\mu^B$ and $\sigma^B$ imply that 

$$
\begin{array}{r l r} \frac {\mu^ {B} - r _ {t}}{\sigma^ {B}} & = & \frac {\frac {\sigma \lambda}{\alpha} (1 - e ^ {- \alpha (s - t)})}{\frac {\sigma}{\alpha} (1 - e ^ {- \alpha (s - t)})} \\ & = & \lambda \end{array}
$$

as expected. Justification for the alterations which make $\mu^B > r_t$ and $\sigma^B > 0$ is provided in Vasicek (Journal of Financial Economics, 1977). Computations which parallel those in the text with 

$$
{ d B } { = } { \mu ^ { B } B d t - \sigma ^ { B } B d W _ { t } }
$$

$$
\begin{array}{r l r} \sigma^ {B} B & = & - b (r _ {t}, t) B _ {r} > 0 \\ \mu^ {B} & = & r _ {t} + \lambda \sigma^ {B} > r _ {t} \end{array}
$$

lead to the intuitive results presented above. These definitions realize apriori that $B_{r}$ is a negative quantity. Overall, with the increment $\Delta W$ approximating $dW_{t}$ , both $-\sigma^{B}B\Delta W$ and $\sigma^{B}B\Delta W$ are distributed $\mathcal{N}\left(0,\left(\sigma^{B}\right)^{2}B^{2}\Delta t\right)$ . Therefore, placing a negative sign in front of $\sigma^{B}$ does not change the distribution of the bond price but results in parameters with greater economic meaning. 

For parts (d) and (e), use the relationship $e^{-\alpha(s-t)} \to 1$ as $t \uparrow s$ . 

(d) Bond price volatility goes to zero as $t \uparrow s$ which is expected since the bond matures at $1 for certain (no default risk is assumed). 

(e) Bond price drift goes to $r_s$ which is also expected. As the bond converges to $1, its return becomes the return of holding $1 over an instant, this is exactly the short term rate. 

(f) $s \uparrow \infty \Rightarrow e^{-\alpha(s-t)} \downarrow 0$ Therefore, the drift on a consult or perpetual bond becomes $r_{t} + \frac{\sigma\lambda}{\alpha}$ and the diffusion parameter becomes $\frac{\sigma}{\alpha}$ . 

2. Two period world with two assets, a savings account (money market) and a bond which pays $1 at maturity ( $t = 2$ ). There are four possible states at $t = 2$ which correspond to the bond price path. For simplicity, denote these four states as $\psi_1 = \psi^{u,u}$ , $\psi_2 = \psi^{u,d}$ , $\psi_3 = \psi^{d,u}$ , and $\psi_4 = \psi^{d,d}$ . 

(a) Form matrix with state prices. 

$$
\left[ \begin{array}{c} 1 \\ B _ {0} \end{array} \right] = \left[ \begin{array}{c c c c} (1 + r _ {0}) (1 + r _ {1}) & (1 + r _ {0}) (1 + r _ {1}) & (1 + r _ {0}) (1 + r _ {1}) & (1 + r _ {0}) (1 + r _ {1}) \\ 1 & 1 & 1 & 1 \end{array} \right] \quad \left[ \begin{array}{c} \psi_ {1} \\ \psi_ {2} \\ \psi_ {3} \\ \psi_ {4} \end{array} \right]
$$

This implies two equations 

(1) 

$$
1 = (1 + r _ {0}) (1 + r _ {1}) \psi_ {1} + (1 + r _ {0}) (1 + r _ {1}) \psi_ {2} + (1 + r _ {0}) (1 + r _ {1}) \psi_ {3} + (1 + r _ {0}) (1 + r _ {1}) \psi_ {4}\tag{2}
$$

$$
B _ {0} = 1 \psi_ {1} + 1 \psi_ {2} + 1 \psi_ {3} + 1 \psi_ {4}
$$

(b) Risk-neutral probabilities can be obtained by setting $\tilde{p}_i = (1 + r_0)(1 + r_1)\psi_i$ $\forall i = 1,2,3,4$ . From the first equation, $\sum_{i=1}^{4}\tilde{p}_i = 1$ , which ensures that a probability measure has been obtained. 

(c) From the second equation and $\psi_{i} = \frac{\tilde{p}_{i}}{(1 + r_{0})(1 + r_{1})}$ 

$$
\begin{array}{r c l} B _ {0} & = & \psi_ {1} + \psi_ {2} + \psi_ {3} + \psi_ {4} \\ & = & \left[ \frac {1}{(1 + r _ {0}) (1 + r _ {1})} \right] \tilde {p} _ {1} + \left[ \frac {1}{(1 + r _ {0}) (1 + r _ {1})} \right] \tilde {p} _ {2} + \left[ \frac {1}{(1 + r _ {0}) (1 + r _ {1})} \right] \tilde {p} _ {3} + \left[ \frac {1}{(1 + r _ {0}) (1 + r _ {1})} \right] \tilde {p} _ {4} \\ & = & E _ {0} ^ {\tilde {P}} \left[ \frac {1}{(1 + r _ {0}) (1 + r _ {1})} \right] \end{array}
$$

Where the last equality follows from the fact that each state has the same payoff, $X(\omega_i) = \left[\frac{1}{(1 + r_0)(1 + r_1)}\right]$ . Thus, $X(\omega_i)$ has no dependence on $\omega_i$ . The expectation $\sum_{i=1}^{4} \tilde{p}_i X(\omega_i)$ reduces to $X \sum_{i=1}^{4} \tilde{p}_i = X$ as the risk-neutral probabilities sum to one according to the first equation. 

## CHAPTER 19

## 1. Consider the two processes

$$
\begin{array}{r c l} r _ {t + \Delta} & = & r _ {t} (1 + \alpha) + \sigma_ {1} (W _ {t + \Delta} - W _ {t}) + \sigma_ {2} (W _ {t} - W _ {t - \Delta}) \\ R _ {t + \Delta} & = & R _ {t} (1 + \beta) + \theta_ {1} (\tilde {W} _ {t + \Delta} - \tilde {W} _ {t}) + \theta_ {2} (\tilde {W} _ {t} - \tilde {W} _ {t - \Delta}) \end{array}
$$

with correlation $E\left[(\Delta \tilde{W})(\Delta W)\right] = \rho \Delta$ 

(a) This error structure is known as a moving average model of order 1 in the time series literature. Both a current “shock” and a previous “shock” enter into the present value of $r_{t}$ . 

Yes, it's plausible that $\Delta W_{t - \Delta} = W_t - W_{t - \Delta}$ may enter into the dynamics of $r_{t + \Delta}$ . For example, if interest rates move up (down) sharply due to some random phenomena, one might expect a possible reversion in the next period. This tendency to mean revert is modeled through two restrictions; $\sigma_1 > 0$ and $\sigma_2 < 0$ . Alternatively, it may be reasonable to assume that interest rates are path dependent. Simply knowing the current value of $r_t$ may not be sufficient for modeling next period's value. In short, interest rates might not necessarily be Markov. 

(b) The closest SDE analogous to this discrete process would be 

$$
d r _ {t} = \alpha r _ {t} d t + \sigma_ {1} d W _ {t}
$$

which is Markov. This SDE fails to account for the second error term. The difficulty is that $r_{t}$ is not Markov, it depends on previous values of the Brownian motion, not just the current movement captured by $dW_{t}$ . 

(c) No, one cannot write a representation for $X_{t}$ such that $X_{t}$ is first order Markov. Even if $\rho = 1$ , $X_{t}$ is still not first order Markov. For $X_{t}$ to be Markov, there must exist some function $f$ such that 

$$
X _ {t + \Delta} = \left(r _ {t + \Delta} R _ {t + \Delta}\right) = f (r _ {t}, R _ {t}) + Z _ {t}
$$

where $Z_{t}$ is the current random variable. In this case, $Z_{t}$ is a function of $\Delta W_{t} = W_{t + \Delta} - W_{t}$ and $\Delta \tilde{W}_t = \tilde{W}_{t + \Delta} - \tilde{W}_t$ , not the previous random disturbances $\Delta W_{t - \Delta} = W_t - W_{t - \Delta}$ and $\Delta \tilde{W}_{t - \Delta} = \tilde{W}_t - \tilde{W}_{t - \Delta}$ . But 

$$
\binom{r _ {t + \Delta}}{R _ {t + \Delta}} = \binom{r _ {t} (1 + \alpha)}{R _ {t} (1 + \beta)} + \left( \begin{array}{c c} \sigma_ {1} & \sigma_ {2} \\ 0 & 0 \end{array} \right) \binom{\Delta W _ {t}}{\Delta W _ {t - \Delta}} + \left( \begin{array}{c c} 0 & 0 \\ \theta_ {1} & \theta_ {2} \end{array} \right) \binom{\Delta \tilde {W} _ {t}}{\Delta \tilde {W} _ {t - \Delta}}
$$

To be first order Markov, the values of $\Delta W_{t - \Delta}$ and $\Delta \tilde{W}_{t - \Delta}$ must be expressed in terms of $R_{t}$ and $r_t$ and not involve $R_{t - \Delta}$ and $r_{t - \Delta}$ or $R_{t + \Delta}$ and $r_{t + \Delta}$ . However, the matrices 

$$
\left( \begin{array}{c c} \sigma_ {1} & \sigma_ {2} \\ 0 & 0 \end{array} \right)
$$

and 

$$
\left( \begin{array}{c c} 0 & 0 \\ \theta_ {1} & \theta_ {2} \end{array} \right)
$$

are not of full rank. Thus, the matrices are not invertible and the values of $\Delta W_{t - \Delta}$ and $\Delta \tilde{W}_{t - \Delta}$ cannot be solved. If $\rho = 1$ , then 

$$
\binom{r _ {t + \Delta}}{R _ {t + \Delta}} = \binom{r _ {t} (1 + \alpha)}{R _ {t} (1 + \beta)} + \left( \begin{array}{c c} \sigma_ {1} & \sigma_ {2} \\ \theta_ {1} & \theta_ {2} \end{array} \right) \binom{\Delta W _ {t}}{\Delta W _ {t - \Delta}}
$$

However, (assume that $\sigma_{1}\theta_{2} - \sigma_{2}\theta_{1}\neq 0$ ), the value for $W_{t - \Delta}$ cannot be expressed in terms of $r_t$ and $R_{t}$ as the following system of equations demonstrates 

$$
\binom{\Delta W _ {t}}{\Delta W _ {t - \Delta}} = \left( \begin{array}{c c} \sigma_ {1} & \sigma_ {2} \\ \theta_ {1} & \theta_ {2} \end{array} \right) ^ {- 1} \binom{r _ {t + \Delta} - r _ {t} (1 + \alpha)}{R _ {t + \Delta} - R _ {t} (1 + \beta)}
$$

Inverting the matrix 

$$
\left( \begin{array}{c c} \sigma_ {1} & \sigma_ {2} \\ \theta_ {1} & \theta_ {2} \end{array} \right)
$$

leaves a dense $2 \times 2$ matrix which implies that any solution for $W_{t - \Delta}$ involves the future short and long term interest rate, not just their present values at time $t$ . Thus, $X_{t}$ is not first order Markov. 

(d) No, the same difficulty in part (b) arises. The past randomness cannot be accounted for in the term $dW_{t}$ . 

(e) Yes, this is possible. Adding another process allows one to condition on more information. In general, the additional information could make the joint process Markov. 

2. (a) A univariate representation for the short rate is 

$$
r _ {t + \Delta} = \alpha_ {1 1} r _ {t} + \alpha_ {1 2} \left[ \sum_ {i = 1} ^ {\infty} \left(\alpha_ {2 1} \alpha_ {2 2} ^ {i - 1} r _ {t - i \Delta} + \alpha_ {2 2} ^ {i} \Delta W _ {t - i \Delta} ^ {2}\right) + \Delta W _ {t} ^ {2} \right] + \Delta W _ {t + \Delta} ^ {1}
$$

provided that $|\alpha_{22}| < 1$ so that the infinite series converge. This equation is the result of a recursion. Expand the matrix into two equations as follows 

$$
{r _ {t + \Delta}} = {\alpha_ {1 1} r _ {t} + \alpha_ {1 2} R _ {t} + \Delta W _ {t + \Delta} ^ {1}}
$$

$$
\begin{array}{r l r} {R _ {t + \Delta}} & = & {\alpha_ {2 1} r _ {t} + \alpha_ {2 2} R _ {t} + \Delta W _ {t + \Delta} ^ {2}} \\ {R _ {t}} & = & {\alpha_ {2 1} r _ {t - \Delta} + \alpha_ {2 2} R _ {t - \Delta} + \Delta W _ {t} ^ {2}} \\ {R _ {t - \Delta}} & = & {\alpha_ {2 1} r _ {t - 2 \Delta} + \alpha_ {2 2} R _ {t - 2 \Delta} + \Delta W _ {t - \Delta} ^ {2}} \\ {\vdots} & & {\vdots} \end{array}
$$

Successive substitution of the past values of $R_{t-i\Delta}$ for $i=0,1,2,\ldots$ into $r_{t+\Delta}$ yields the solution. 

(b) According to this representation, $r_{t}$ is not a Markov process. Infinitely many past values of the random “shocks” and the spot rate process are required to represent $r_{t}$ . 

(c) The univariate process for $r_t$ would be Markov if $\alpha_{12} = 0$ . In this case, $r_{t + \Delta} = \alpha_{11}r_t + \Delta W_{t + \Delta}^1$ . 

3. (a) There are $2^{3} = 8$ possible states of the world at time $t = 3$ . 

(b) Portfolio 1: 

<table><tr><td>Position</td><td>Cash flows at 0</td><td>Cash flows at 1</td></tr><tr><td>Long the forward, <eq>f_0</eq></td><td>+$1.0000</td><td>-$1.0800</td></tr><tr><td>Long 1.08 units of the <eq>B_1</eq> bond</td><td>-$0.9720</td><td>+$1.0800</td></tr><tr><td>Net cash flows</td><td>+$0.0280</td><td>$0.0000</td></tr></table>

Portfolio 2: 

<table><tr><td>Position</td><td>Cash flows at 0</td><td>Cash flows at 1</td><td>Cash flows at 2</td></tr><tr><td>Short 1.09 units of <eq>B_{2}</eq> bond</td><td>+\$0.9483</td><td>\$0.0000</td><td>-\$1.0900</td></tr><tr><td>Long the <eq>B_{1}</eq> bond</td><td>-\$0.9000</td><td>+\$1.0000</td><td>\$0.0000</td></tr><tr><td>Short the forward, <eq>f_{1}</eq></td><td>\$0.0000</td><td>-\$1.0000</td><td>+\$1.0900</td></tr><tr><td>Net cash flows</td><td>+\$0.4830</td><td>\$0.0000</td><td>\$0.0000</td></tr></table>

Portfolio 3: 

<table><tr><td>Position</td><td>Cash flows at 0</td><td>Cash flows at 2</td><td>Cash flows at 3</td></tr><tr><td>Short 1.1 units of <eq>B_{3}</eq> bond</td><td>+\$0.9020</td><td>\$0.0000</td><td>-\$1.1000</td></tr><tr><td>Long the <eq>B_{2}</eq> bond</td><td>-\$0.8700</td><td>+\$1.0000</td><td>\$0.0000</td></tr><tr><td>Short the forward, <eq>f_{2}</eq></td><td>\$0.0000</td><td>-\$1.0000</td><td>+\$1.1000</td></tr><tr><td>Net cash flows</td><td>+\$0.0320</td><td>\$0.0000</td><td>\$0.0000</td></tr></table>

$$
B _ {n} = \frac {1}{1 + f _ {0}} \frac {1}{1 + f _ {1}} \frac {1}{1 + f _ {2}} \dots \frac {1}{1 + f _ {n - 1}}.\tag{c}
$$

This follows from the fact that to avoid arbitrage opportunities, the forward rates must satisfy $f_{i} = \frac{B_{i}}{B_{i+1}} - 1$ . This relationship implies that $B_{n} = \frac{B_{n-1}}{1 + f_{n-1}}$ but $B_{n-1} = \frac{B_{n-2}}{1 + f_{n-2}}$ which implies that $B_{n} = \frac{B_{n-2}}{1 + f_{n-2}} \frac{1}{1 + f_{n-1}}$ and so forth until the right hand side only involves $B_{0} = 1$ . 

(d) Combinations of the above portfolios can generate an infinite number of possible returns. 

(e) No, the $B_{i}$ 's cannot be determined independently. All bond prices are derived from the same underlying term structure. 

(f) No, the $f_{i}$ 's cannot be determined independently either. The forward rates are implied from bond prices and are found recursively. The forward rate $f_{i}$ depends on previous forward rates, for instance, $f_{i-1}$ . 

(g) Presently, only asymptotically are the $f_{i}$ 's normally distributed. The $f_{i}$ 's are a discrete process taking, at most, 8 possible values. Theoretically, modeling bonds and the forward rates as a normal process allows for negative values. This consequence has no economic rationale and implies the existence of arbitrage opportunities. 

4. (a) Find the measure under which the discounted bond process is a martingale. Then, take the expectation of the payoff under this measure. 

(b) See part (c) for an assessment of the assumptions. 

(c) The first assumption is not appropriate under the risk - neutral measure since the expectation of $L_{i}$ under this measure is not equal to $f_{i}$ . The second assumption is not reasonable as the $f_{i}$ 's cannot have mean 0 since they do not take on non - positive values. 

(d) As for the first assumption, this becomes reasonable under the forward measure since $f_{i} = E_{f}(L_{i})$ , the expectation of $L_{i}$ under the forward measure. However, using the forward measure does not make the $2^{nd}$ assumption any more reasonable. 

(e) As mentioned above, since $f_{i} = E_{f}(L_{i})$ the forward measure $p_{1}$ satisfies 

$$
{f _ {1}} = {E _ {f} (L _ {i}) = p _ {1} L _ {1} ^ {u} + (1 - p _ {1}) L _ {1} ^ {d}}
$$

$$
\Rightarrow p _ {1} = \frac {f _ {1} - L _ {1} ^ {d}}{L _ {1} ^ {u} - L _ {1} ^ {d}}
$$

For the forward measure at $t = 2$ , $p_2^u$ and $p_2^d$ satisfy 

$$
{f _ {2}} = {p _ {1} p _ {2} ^ {u} L _ {2} ^ {u u} + p _ {1} (1 - p _ {2} ^ {u}) L _ {2} ^ {u d} + (1 - p _ {1}) p _ {2} ^ {d} L _ {2} ^ {d u} + (1 - p _ {1}) (1 - p _ {2} ^ {d}) L _ {2} ^ {d d}}
$$

$$
{ 1 } { = } { p _ { 1 } p _ { 2 } ^ { u } + p _ { 1 } ( 1 - p _ { 2 } ^ { u } ) + ( 1 - p _ { 1 } ) p _ { 2 } ^ { d } + ( 1 - p _ { 1 } ) ( 1 - p _ { 2 } ^ { d } ) }
$$

where $p_{2}^{d}$ is the probability of the spot rate process moving from $L_{1}^{d}$ to $L_{2}^{du}$ . Thus, given the dynamics of the spot process, the forward measure is recoverable with two unknowns, $p_{2}^{u}$ and $p_{2}^{d}$ , and two equations. The first equation states that the forward rate is the expected future spot rate while the second equation merely assets that the sum of the probabilities at t=2 equals one. 

(f) The price of the option is then given by 

$$
C _ {0} = B (0, 2) \left[ p _ {1} p _ {2} ^ {u} C (2, u u) + p _ {1} (1 - p _ {2} ^ {u}) C (2, u d) + (1 - p _ {1}) p _ {2} ^ {d} C (2, d u) + (1 - p _ {1}) (1 - p _ {2} ^ {d}) C (2, d d) \right]
$$

Note that the forward measure employs $B(0,2)$ and not the money market account. The forward measures uses a different numeraire, a bond instead of the money market, for normalizing assets in the economy. 

## CHAPTER 20

1. Consider the process $dr_{t} = \sigma r_{t} dW_{t}$ with $r_{0} = .05$ . 

(a) The spot rate dynamics are a martingale under the empirical measure as there is no drift term in the SDE. 

(b) With $a(r_{t},t)=0$ and $b(r_{t},t)=\sigma r_{t}$ , the PDE for the bond price $B(t,T)$ becomes 

$$
r _ {t} B = B _ {t} - B _ {r} \lambda (r _ {t}, t) \sigma r _ {t} + \frac {1}{2} B _ {r r} \sigma^ {2} r _ {t} ^ {2}
$$

where $\lambda(r_{t},t)$ represents the market price of risk. 

(c) A solution to this PDE is $B(t,T) = E_{t}^{P}\left[e^{-\int_{t}^{T}r_{s}ds + \int_{0}^{t}\lambda (r_{s},s)dW_{s} - \frac{1}{2}\int_{0}^{t}\lambda^{2}(r_{s},s)ds}\right]$ . Use the SDE given in the problem to conclude that 

$$
r _ {s} = r _ {t} e ^ {\sigma (W _ {s} - W _ {t}) - \frac {\sigma^ {2}}{2} (s - t)}
$$

for verification. 

(d) The market price of risk equals $\frac{\mu_{i}-r}{\sigma_{i}}$ where $\mu_{i}$ and $\sigma_{i}$ are the drift and volatility of the bond. This market price of risk is the compensation investors require to hold bonds since they are exposed to term structure risk in the form of $W_{t}$ . This premium is positive. The denominator, $\sigma_{i}$ , is always positive. The numerator is also positive since $\mu_{i}>r$ . This inequality is intuitive. Imagine if it did not hold, $\mu_{i}<r$ . Then the expected return on a particular bond would be less than the risk-free rate. No one would be interested in holding such a bond. 

2. Consider the mean reverting spot rate model $dr_{t} = \alpha(\kappa - r_{t})dt + bdW_{t}$ introduced by Vasicek. 

(a) Let $B(t,T)$ be represented as $B$ with $B_{x}$ denoting the partial derivative of the bond price with respect to the variable $x$ . An SDE for the bond price dynamics follows from Ito's lemma. 

$$
\begin{array}{r c l} {d B} & {=} & {\left(B _ {t} + B _ {r} a (r _ {t}, t) + \frac {1}{2} B _ {r r} b ^ {2} (t, r _ {t})\right) d t + B _ {r} b (r _ {t}, t) d W _ {t}} \\ & {=} & {\left(B _ {t} + B _ {r} \left[ a (r _ {t}, t) - b (r _ {t}, t) \lambda_ {t} \right] + \frac {1}{2} B _ {r r} b ^ {2} (t, r _ {t})\right) d t + B _ {r} b (r _ {t}, t) d \tilde {W} _ {t}} \\ & {=} & {\left(B _ {t} + B _ {r} \left[ \alpha (\kappa - r _ {t}) - b \lambda_ {t} \right] + \frac {1}{2} B _ {r r} b\right) d t + B _ {r} b d \tilde {W} _ {t}} \end{array}
$$

(b) For the drift and diffusion parameters, see the calculations in chapter 18, problem 1, part (c). Simply replace $\sigma$ with $b$ . 

(c) Yes, this is expected. Girsanov's theorem changes the mean but not the diffusion component of an SDE. Under the risk - neutral measure, the drift on the SDE has been altered but not the diffusion component. 

(d) As maturity approaches, $t \uparrow T$ , the diffusion of the bond approaches zero. This is intuitive since the bond matures at face value. The final value of the bond is known. 

(e) The risk premium $\mu - r$ does not depend on the volatility of the bond. However, the market price of risk is proportional to the risk premium. The market price of risk is simply the risk premium standardized by the volatility of the bond. These relationships are important as they allow Girsanov's theorem to alter the drift (through the risk premium) but not the volatility of the bond price SDE under a change of measure. 

(f) As in chapter 18, the drift of the bond approaches $r_t + \frac{b\lambda}{\alpha}$ while the volatility of the bond approaches $\frac{b}{\alpha}$ . 

(g) The yield of a bond, $R(t,T)$ , equals 

$$
R (t, T) = - \frac {1}{T} \ln B (t, t + T)
$$

With the bond price given in the problem 

$$
R = \lim _ {T \to \infty} R (t, T) = \kappa + \frac {b \lambda}{\alpha} - \frac {b ^ {2}}{2 \alpha^ {2}}
$$

Therefore, R represents the yield on a consul bond with infinite maturity. 

## CHAPTER 21

1. Define the Radon Nikodym as $V(t,T) = e^{\int_t^T\lambda (r_s,s)dW_s - \frac{1}{2}\int_t^T\lambda^2 (r_s,s)ds}$ (a martingale provided that $\lambda (r_s,s)$ is square integrable by Novikov's criterion). This quantity is responsible for changing the bond process to the equivalent martingale measure. 

(a) Let $B(t,T) = E_{t}^{\tilde{P}}\left[e^{-\int_t^T r_s ds}\right]$ . The Ito product rule implies 

$$
B (t, T) V (t, T) = B (0, T) V (0, T) + \int_ {0} ^ {t} B (s, T) d V (s, T) + \int_ {0} ^ {t} V (s, T) d B (s, T) + \langle B (s, T), V (s, T) \rangle_ {t}
$$

Since $B(t,T)$ is of bounded variation, the quadratic variation between the two processes is zero and the last term may be omitted. 

$$
B (t, T) V (t, T) = B (0, T) V (0, T) + \int_ {0} ^ {t} B (s, T) d V (s, T) + \int_ {0} ^ {t} V (s, T) d B (s, T)
$$

Therefore, the standard product rule may be applied 

$$
\begin{array}{r c l} d (B (t, T) V (t, T)) & = & d B (t, T) V (t, T) + B (t, T) d V (t, T) \\ & = & r (t) B (t, T) V (t, T) d t - \lambda (r _ {t}, t) B (t, T) V (t, T) d W _ {t} \\ & = & B (t, T) V (t, T) [ r (t) d t - \lambda (r _ {t}, t) d W _ {t} ] \end{array}
$$

(b) Obtaining an expression for $dB(t,T)$ is accomplished by observing that $b(r_t,t) = \sigma$ and $a(r_t,t) = \mu$ . From the previous section 

$$
{ d B } { = } { \left[ B _ { t } + ( \mu - \lambda \sigma ) B _ { r } + \frac { 1 } { 2 } B _ { r r } \sigma ^ { 2 } \right] d t + \sigma B _ { r } d \tilde { W } _ { t } }
$$

$$
\begin{array}{r c l} \frac {B (t , T)}{B (t)} & = & E _ {t} ^ {\tilde {P}} \left[ \frac {B (T , T)}{B (T)} \right] \qquad \mathrm{martingaleproperty} \\ & = & E _ {t} ^ {\tilde {P}} \left[ \frac {1}{B (T)} \right] \qquad \mathrm{since} B (T, T) = 1 (\mathrm{zerocouponbondmaturingat$1}) \\ \Rightarrow B (t, T) & = & E _ {t} ^ {\tilde {P}} \left[ \frac {B (t)}{B (T)} \right] \qquad \mathrm{since} B (t) \mathrm{isadaptedto} \mathcal {F} _ {t} \\ & = & E _ {t} ^ {\tilde {P}} \left[ e ^ {- \int_ {t} ^ {T} r _ {s} d s} \right] \\ & = & E _ {t} ^ {P} \left[ e ^ {- \int_ {t} ^ {T} r _ {s} d s} V (t, T) \right] \end{array}
$$

More justification is possible using the result of part (a). Manipulate the SDE to form 

$$
\frac {d (B (t , T) V (t , T))}{B (t , T) V (t , T)} = - \left[ - r (t) d t + \lambda (r _ {t}, t) d W _ {t} \right]
$$

The solution to this SDE parallels earlier results for the stock price. 

$$
\begin{array}{r c l} \frac {d S (t)}{S (t)} & = & r (t) d t + \sigma (t) d W (t) \\ \Rightarrow S (t) & = & e ^ {\int_ {0} ^ {t} r _ {s} d s + \int_ {0} ^ {t} \sigma (s) d W _ {s} - \frac {1}{2} \int_ {0} ^ {t} \sigma^ {2} (s) d s} \end{array}
$$

In the context of this question, the solution to the SDE is 

$$
{ B ( T , T ) V ( T , T ) } { = } { B ( t , T ) V ( t , T ) e ^ { - \left[ - \int _ { t } ^ { T } r _ { s } d s + \int _ { t } ^ { T } \lambda ( r _ { s } , s ) d W _ { s } - \frac { 1 } { 2 } \int _ { t } ^ { T } \lambda ^ { 2 } ( r _ { s } , s ) d s \right] } }
$$

The left hand side terms $V(T,T)$ and $B(T,T)$ both equal one by definition. Taking the exponential terms on the right hand side over to the left hand side results in 

$$
e ^ {- \int_ {t} ^ {T} r _ {s} d s + \int_ {t} ^ {T} \lambda (r _ {s}, s) d W _ {s} - \frac {1}{2} \int_ {t} ^ {T} \lambda^ {2} (r _ {s}, s) d s} = B (t, T) V (t, T)
$$

After taking expectations under measure P at time t, the right hand side becomes $E_{t}^{P}\left[B(t,T)V(t,T)\right]=B(t,T)E_{t}^{\tilde{P}}\left[1\right]=B(t,T)$ . The final result is 

$$
B (t, T) = E _ {t} ^ {P} \left[ e ^ {- \int_ {t} ^ {T} r _ {s} d s + \int_ {t} ^ {T} \lambda (r _ {s}, s) d W _ {s} - \frac {1}{2} \int_ {t} ^ {T} \lambda^ {2} (r _ {s}, s) d s} \right]
$$

## CHAPTER 22

1. (a) For independent random variables, $E\left(\prod_{i=1}^{n} X_i\right) = \prod_{i=1}^{n} E(X_i)$ . Therefore 

$$
\begin{array}{r c l} E \left(\prod_ {t = 1} ^ {T} (z _ {t} + 1)\right) & = & \prod_ {t = 1} ^ {T} E (z _ {t} + 1) \\ & = & \prod_ {t = 1} ^ {T} 1 \\ & = & 1. \end{array}
$$

This is independent of T. 

(b) It is not clear when it is best to stop the game. If one uses expected reward as the criterion for optimal stopping, then it does not matter what the stopping rule is. All stopping rules yield the same expected reward. However, using the expected reward as the optimal stopping criterion implicitly assumes that one can play this many times over the long run. If one has only a single chance to play the game, another criterion may be in order. 

$$
\begin{array}{r l r} {E \left(\frac {2 T _ {k}}{T _ {k + 1}} \prod_ {t = 1} ^ {T _ {k}} (z _ {t} + 1)\right)} & = & {\frac {2 k}{k + 1} E \left(\prod_ {t = 1} ^ {k} (z _ {t} + 1)\right)} \\ & = & {\frac {2 k}{k + 1}.} \end{array}\tag{c}
$$

This follows since $T_{k}$ is deterministic. 

(d) The expected reward is increasing in $T_{k}$ . Thus, the expected reward is maximized as $k \to \infty$ . 

(e) Again, if one chooses the optimal stopping rule to maximize the expected reward, then the optimal rule would be to never stop. However, this by definition is not a stopping rule, meaning an optimal stopping rule does not exist. 

2. (a) At time $T + 1$ , assuming the reward is not already 0, one of 2 things can happen; either the reward goes to 0, or the reward becomes $\frac{(T + 1)2^{T + 2}}{(T + 2)}$ . Thus, conditional on $W_{T} = w_{T}^{*}$ 

$$
\begin{array}{r c l} E (W _ {T + 1} | W _ {T} = w _ {t} ^ {*}) & = & 0 \times \frac {1}{2} + \frac {(T + 1) 2 ^ {T + 2}}{(T + 2)} \times \frac {1}{2} \\ & = & \frac {(T + 1) 2 ^ {T + 1}}{(T + 2)}. \end{array}
$$

(b) This expected value is larger than $W_{T}$ . Thus, the player should never stop when only considering expected value. 

(c) For any given game, the game will end with probability one, $P(z_{t} = -1, t < \infty) = 1$ . If a player decides to never stop, then the game will eventually end after a “tails”. This leaves the player with no winnings. 

(d) As alluded to above, for any given game, the game will end with probability one. Thus, a paradox appears. If a player wants to maximize expected winnings, then the player should never stop. However, with certainty, this strategy leaves the player with nothing. 

(e) The criterion one uses to determine the stopping time is expected winnings. This criterion is suitable if one can play the game infinitely often. However, when one has a limited number of trials, a different stopping criterion may be desirable. 

The expected reward for stopping at time T is increasing in T because the reward grows larger and larger. However, the probability of such a reward is also being reduced. Thus, although the expected reward becomes larger as the stopping time increases, the probability of actually getting that reward diminishes. 

3. Pricing an American call option requires checking each node of the tree to determine if the intrinsic value (immediate value if exercised) is greater than the value computed by waiting an additional time period. 

(a) Let $\Delta = \frac{200}{4} = 50$ days or $\frac{50}{365}$ . Therefore, $u$ equals $e^{\sigma \sqrt{\Delta}} = e^{.12\sqrt{\frac{50}{365}}} = 1.0454$ and $d$ equals $\frac{1}{u} = .9566$ . 

(b) The risk-neutral implied up probability is $\frac{1 + (.06)\left(\frac{50}{365}\right) - .9566}{1.0454 - .9566} = .5814$ . 

(c) stock price tree: 

$$
t = 0 \quad t = 1 \quad t = 2 \quad t = 3 \quad t = 4
$$

$$
\begin{array}{c c c c c} & & & & 1 1 9. 4 4 \\ & & & 1 1 4. 2 5 \\ & & 1 0 9. 2 9 & & 1 0 9. 2 9 \\ & 1 0 4. 5 4 & & 1 0 4. 5 4 \\ 1 0 0 & & 1 0 0 & & 1 0 0 \\ & 9 5. 6 6 & & 9 5. 6 6 \\ & & 9 1. 5 0 & & 9 1. 5 0 \\ & & & 8 7. 5 3 & \\ & & & & 8 3. 7 2 \end{array}
$$

(d) call price tree: 

Intrinsic value (immediate exercise) simply subtracts the strike price of 100 from each node of the stock price tree if the stock price is above 100 at that node. Otherwise, the value at that node is set to zero. 

$$
\begin{array}{c c c c c} t = 0 & t = 1 & t = 2 & t = 3 & t = 4 \\ & & & & 1 9. 4 4 \\ & & & 1 4. 2 5 \\ & & 9. 2 9 & & 9. 2 9 \\ & 4. 5 4 & & 4. 5 4 \\ 0 & & 0 & & 0 \\ & 0 & & 0 \\ & & 0 & & 0 \\ & & & 0 \end{array}
$$

Compare the intrinsic value with the usual procedure of discounting the call values starting from t = 4. 

$$
\begin{array}{c c c c c} t = 0 & t = 1 & t = 2 & t = 3 & t = 4 \\ & & & & 1 9. 4 4 \\ & & & 1 5. 0 7 \\ & & 1 0. 9 2 & & 9. 2 9 \\ & 7. 5 8 & & 5. 3 6 \\ 5. 1 5 & & 3. 0 9 & & 0 \\ & 1. 7 8 & & 0 \\ & & 0 & & 0 \\ & & & 0 \end{array}
$$

The nodes of the second tree have call values which are always higher than those produced by exercising the option before maturity. Therefore, one would never exercise the option before maturity and $5.15 is the price of the option. Since one does not exercise the option early, one can invoke the Black Scholes formula which generated a call price of $5.34. The binomial approximation with just 4 steps performed reasonably well. 

(e) One would never exercise the option early as the value of waiting and discounting next period's expected value is higher at every possible node. 

4. Early exercise with dividends. After a dividend, the stock value decreases. This may result in early exercise of an American option prior to a dividend payout. It is assumed that if an option were to be exercised at an intermediate node, the option would be exercised prior to any dividend being paid. 

(a) A $4\%$ continuous dividend does not effect the values of $u$ and $d$ but it does alter the implied probability. In this case, $p$ equals $\frac{1 + (r - \delta)\left(\frac{50}{365}\right) - d}{u - d} = .5197$ which is lower than in problem 3 as the dividend decreases the probability that the stock increases next period. The stock price tree is identical but the expected value of the call option on the intermediate nodes changes as follows 

$$
\begin{array}{c c c c c} t = 0 & t = 1 & t = 2 & t = 3 & t = 4 \\ & & & & 1 9. 4 4 \\ & & & 1 4. 4 5 \\ & & 9. 7 3 & & 9. 2 9 \\ & 6. 1 9 & & 4. 7 9 \\ 3. 8 0 & & 2. 4 7 & & 0 \\ & 1. 2 7 & & 0 \\ & & 0 & & 0 \\ & & & 0 \end{array}
$$

The intrinsic value from the previous question has not changed since the stock price tree has not changed. By inspection, each node on the above tree is higher than the value of immediately exercising the option. Therefore, with this continuous dividend, one would still never exercise early. However, the dividend does reduce the value of the call option to $3.80. This value is close to the Black Scholes value (European option calculation valid as one exercises only at maturity) of $4.01. 

(b) The stock pays 5% of its value at the third node. Here, the stock price tree at t = 3 and t = 4 does change to account for the dividend. Despite the dividend at the third node, the tree still recombines. For a given S, the up node next period has a value of $\frac{Su}{1.05}$ while the value at the bottom node next period is $\frac{Sd}{1.05}$ . Therefore, after an up and down movement or a down and then up movement, the stock price recombines, $\frac{Su}{1.05}d = \frac{Sd}{1.05}u = \frac{S}{1.05}$ . The values of u and d have not changed which allows new terminal values to be computed. 

stock price tree (after dividend at $t = 3$ ): 

$$
\begin{array}{c c c c c} t = 0 & t = 1 & t = 2 & t = 3 & t = 4 \\ & & & & 1 1 3. 7 5 \\ & & & 1 0 8. 8 1 \\ & & 1 0 9. 2 9 & & 1 0 4. 0 8 \\ & 1 0 4. 5 4 & & 9 9. 5 6 \\ 1 0 0 & & 1 0 0 & & 1 0 0 \\ & 9 5. 6 6 & & 9 1. 1 0 \\ & & 9 1. 5 0 & & 8 7. 1 5 \\ & & & 8 3. 3 6 \\ & & & & 7 9. 7 4 \end{array}
$$

The intrinsic value of the option is almost identical to the option in problem 3 except at the terminal nodes. The values at t = 3 are identical since one would exercise just prior to the dividend being paid to avoid a decrease in the stock price. Therefore, the dividend would only reduce the intrinsic value of the option at t = 4. 

$$
\begin{array}{c c c c c} t = 0 & t = 1 & t = 2 & t = 3 & t = 4 \\ & & & & 1 3. 7 5 \\ & & & 1 4. 2 5 \\ & & 9. 2 9 & & 4. 0 8 \\ & 4. 5 4 & & 4. 5 4 \\ 0 & & 0 & & 0 \\ & 0 & & 0 \\ & & 0 & & 0 \\ & & & 0 \end{array}
$$

lxxxvi 

When one works backward at t = 3 to compute the value of waiting to exercise the option at t = 4, the values of 

$$
9. 6 2 = \frac {1 3 . 7 5 p + 4 . 0 8 (1 - p)}{1 + (. 0 6) \left(\frac {5 0}{3 6 5}\right)} <   1 4. 2 5
$$

and 

$$
2. 3 5 = \frac {4 . 0 8 p + 0 (1 - p)}{1 + (. 0 6) \left(\frac {5 0}{3 6 5}\right)} <   4. 5 4
$$

are computed. The value of p is from problem 3 since continuous dividends are no longer being paid in this example. Both these values are less than their counterparts on the intrinsic value tree (14.25 and 4.54). Thus, one would exercise early at t = 3 and not allow the dividend to reduce the stock price before exercising the option. 

call price tree (exercise at t = 3): 

$$
\begin{array}{c c c c} t = 0 & t = 1 & t = 2 & t = 3 \\ & & & 1 4. 2 5 \\ & & 1 0. 1 0 \\ & 6. 9 1 & & 4. 5 4 \\ 4. 6 1 & 1. 5 1 & 2. 6 2 \\ & & 0 \\ & & & 0 \end{array}
$$

Before t = 3, it is best not to exercise the option. The discounted expected value of the option is greater than the intrinsic value at each node prior to t = 3. 

(c) Dividend of $5 paid at time $t = 3$ . Now the tree no longer recombines. The value of a stock after an up and down movement no longer equals the value of the stock after a down and then up movement. There is path dependence since $(Su - 5)d \neq (Sd - 5)u$ . In fact, since $5d < 5u$ , the down and then up movement is always less than an up and then down movement. 

stock price tree (dividend at $t = 3$ ): 

$$
\begin{array}{c c c c c} t = 0 & t = 1 & t = 2 & t = 3 & t = 4 \\ & & & & 1 1 4. 2 1 \\ & & & 1 0 9. 2 5 \\ & & & & 1 0 4. 5 0 \\ & & 1 0 9. 2 9 & & 1 0 4. 0 6 \\ & 1 0 4. 5 4 & & 9 9. 5 4 \\ & & & & 9 5. 2 2 \\ 1 0 0 & & 1 0 0 & & 9 4. 7 8 \\ & 9 5. 6 6 & & 9 0. 6 6 \\ & & & & 8 6. 7 2 \\ & & 9 1. 5 0 & & 8 6. 2 8 \\ & & & 8 2. 5 3 \\ & & & & 7 8. 9 4 \end{array}
$$

Only at t = 4 does the intrinsic value change when compared to part (b) since one could exercise the option at t = 3 prior to any dividend being paid. 

$$
\begin{array}{c c c c c} t = 0 & t = 1 & t = 2 & t = 3 & t = 4 \\ & & & & 1 4. 2 1 \\ & & & 1 4. 2 5 \\ & & & & 4. 5 0 \\ & & 1 0 9. 2 9 & & 4. 0 6 \\ & 4. 5 4 & & 4. 5 4 \\ & & & & 0 \\ 0 & & 0 & & 0 \\ & 0 & & 0 \\ & & & & 0 \\ & & 0 & & 0 \\ & & & 0 \\ & & & & 0 \end{array}
$$

As in part (b), the discounted expected value of the option at $t = 3$ , assuming the option is exercised at $t = 4$ , is less than the intrinsic value at both relevant nodes. 

$$
\begin{array}{r l r} {1 0. 0 6} & = & {\frac {1 4 . 2 1 p + 4 . 5 0 (1 - p)}{1 + (. 0 6) \left(\frac {5 0}{3 6 5}\right)} <   1 4. 2 5} \\ {2. 3 4} & = & {\frac {4 . 0 6 p}{1 + (. 0 6) \left(\frac {5 0}{3 6 5}\right)} <   4. 5 4} \end{array}
$$

Therefore, exercise the option at t = 3 and then proceed to discount the expected call option values backwards in time. These values are greater than the intrinsic values presented above from t = 0 to t = 2 inclusive. 

call price tree (exercise at $t = 3$ ): 

$$
\begin{array}{c c c c} t = 0 & t = 1 & t = 2 & t = 3 \\ & & & 1 4. 2 5 \\ & & 1 0. 1 0 \\ & 6. 9 1 & & 4. 5 4 \\ 4. 6 1 & & 2. 6 2 \\ & 1. 5 1 & & 0 \\ & & 0 & \\ & & & 0 \end{array}
$$

Therefore, despite different dividend policies, the options in parts (b) and (c) have the same value. This is explained by the fact that one would exercise prior to either dividend being paid at t = 3. The call values of $4.61 are less than $5.15 calculated in problem 3 since it was not optimal to exercise early in problem 3. The dividends forced the option holder to exercise one period earlier. In the absence of dividends, the option holder would have exercised only at maturity if the option was in-the-money. 

5. This problem is solved using dynamic programming. Some modifications are made to the original question. The process begins at t = 4 and finds the optimal instrument $k_{4}$ . Then, it proceeds backwards in time to find the optimal instruments $k_{3}$ , $k_{2}$ , and $k_{1}$ . These values and the initial condition $Y_{0} = 0$ generate the values of $Y_{1}, \ldots, Y_{4}$ and the corresponding values of the objective function through time. 

$$
t = 4:
$$

$$
\begin{array}{r l} \text {maximize} & 2 (k _ {4} - k _ {3}) ^ {2} + 1 0 0 (Y _ {4}) ^ {2} \text {with respect to} k _ {4} \\ \text {subject to:} & Y _ {4} = . 2 k _ {4} +. 6 Y _ {3} \end{array}
$$

is equivalent to maximizing 

$$
2 (k _ {4} - k _ {3}) ^ {2} + 1 0 0 (. 2 k _ {4} +. 6 Y _ {3}) ^ {2}
$$

or 

$$
- 2 (k _ {4} - k _ {3}) ^ {2} + (2 k _ {4} + 6 Y _ {3}) ^ {2}
$$

with respect to $k_{4}$ after substituting the $Y_{4}$ constraint into the first expression. However, this function, for fixed $k_{3}$ and $Y_{3}$ , is monotonically increasing in $k_{4}$ . Therefore, the solution would be to choose $k_{4} = \infty$ . Therefore, change the sign of the first term to $-2(k_{4} - k_{3})^{2}$ . This functional form penalizes the policy maker for choosing an instrument path with a high degree of variability. In a financial context, a form of “transaction costs” are imposed as a smooth instrument path is desired. However, even this modification is not sufficient since 

$$
- 2 (k _ {4} - k _ {3}) ^ {2} + (2 k _ {4} + 6 Y _ {3}) ^ {2}
$$

has $2k_{4}^{2}$ as a leading term. Therefore, the function is still monotonically increasing in $k_{4}$ . Alter the objective function once more to 

$$
\begin{array}{r l} \text {maximize} & \sum_ {t = 1} ^ {4} - 2 (k _ {t} - k _ {t - 1}) ^ {2} + 1 0 (Y _ {t}) ^ {2} \\ \text {subject to:} & Y _ {t} = . 2 k _ {t} +. 6 Y _ {t - 1} \end{array}
$$

In this formulation, less weight is given to the target variable $Y_{t}$ which contains $k_{4}$ . Investing an infinite amount in the instrument is no longer optimal. 

(a) At $t = 4$ : 

$$
\begin{array}{r l} \text {maximize} & - 2 (k _ {4} - k _ {3}) ^ {2} + 1 0 (Y _ {4}) ^ {2} \text {with respect to} k _ {4} \\ \text {subject to:} & Y _ {4} = . 2 k _ {4} +. 6 Y _ {3} \end{array}
$$

or 

$$
\mathrm{At} t = 4:
$$

$$
\mathrm{maximize} \qquad - 2 (k _ {4} - k _ {3}) ^ {2} + 1 0 (. 2 k _ {4} +. 6 Y _ {3}) ^ {2} \mathrm{withrespectto} k _ {4}
$$

Taking the partial derivative with respect to $k_{4}$ and setting the result to zero yields 

$$
- 4 (k _ {4} - k _ {3}) + 4 (. 2 k _ {4} +. 6 Y _ {3}) = 0
$$

Therefore 

$$
k _ {4} = \frac {k _ {3} + . 6 Y _ {3}}{. 8}
$$

Taking the second derivative ensures that a maximum has been found 

$$
\frac {\partial^ {2} \left(- 2 (k _ {4} - k _ {3}) ^ {2} + 1 0 (. 2 k _ {4} + . 6 Y _ {3}) ^ {2}\right)}{(\partial k _ {4}) ^ {2}} = - \frac {3 2}{1 0} <   0
$$

(b) see “Instrument” entry in table below 

(c) see “Instrument” entry in table below 

(d) see "Value" entry in table below 

Continuing this procedure from t=3 to t=1 reveals that $k_{t}=\frac{k_{t-1}+.6Y_{t-1}}{.8}$ . Therefore, in addition to $Y_{0}=0$ , the initial value $k_{0}$ is needed. Let $k_{0}=1$ . These values imply that $k_{1}$ and hence $Y_{1}$ can be solved as $k_{1}=1.25$ and $Y_{1}=.2(1.25)+.6(0)=.25$ . Thus, the value function at t=1 equals $-2(.25)^{2}+10(.25)^{2}=.5$ . Moving forward in time, the following table summarizes the results 

<table><tr><td>Time</td><td>Instrument</td><td>Target</td><td>Value</td></tr><tr><td>0</td><td>1.00</td><td>0</td><td>not defined</td></tr><tr><td>1</td><td>1.25</td><td>.25</td><td>.50</td></tr><tr><td>2</td><td>1.75</td><td>.50</td><td>2.00</td></tr><tr><td>3</td><td>2.56</td><td>.81</td><td>5.28</td></tr><tr><td>4</td><td>3.81</td><td>1.25</td><td>12.50</td></tr></table>

(e) Plot of the value function. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5882bd1f-b733-4ed9-8bdc-4c98ae290af0/e3e767090851ff0f7962990b8af425209b15ff121ad1f70a9a8e60f97d60ae0a.jpg)



FIGURE 0.16 Value Function over Time with Optimal Instruments


Both the instrument and the target variable increase in a steady manner over time. The instrument does not increase rapidly as a penalty is imposed on the value function to prevent a trivial solution. Overall, the value function increases along with the instrument and target variable. 