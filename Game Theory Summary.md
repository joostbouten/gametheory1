# Game Theory I
---

Required for the exam:

Slides 1 -- 56 & 70 -- 155

**Chapter 1:** Static games with complete information (normal form)

*Static:* every player moves only once

*Complete information:* each player knows the payoff of all players

A _normal form game_ $(\ \Gamma_N)$ has:

- Players $1, ..., I$
- Strategy spaces $S_i$
- Strategy profiles $s=(s_1, ...,s_I)$, where $s_i \in S_i$
- Payoff functions $u_i(s_1, ...,s_I)$

-
$s_i\in S_i$ Is a *strictly dominant strategy* if for all $s_i\ne s'_i$ we have $u_i(s_i,s_{-i})>u_i(s'_i,s_{-i})$ for all $s_{-i}\in S_{-i}$

-



-
$s_i\in S_i$ Is a *strictly dominated strategy* if there exists another strategy $s'_i\in S_i$ such that $u_i(s_i',s_{-i})>u_i(s_i,s_{-i})$ for all $s_{-i}\in S_{-i}$

-

-
$s_i\in S_i$ Is a *weakly dominated strategy* if there exists another strategy $s'_i\in S_i$ such that $u_i(s_i',s_{-i})\ge u_i(s_i,s_{-i})$ for all $s_{-i}\in S_{-i}$ and $u_i(s_i',s_{-i})>u_i(s_i,s_{-i})$ for at least one $s_{-i}\in S_{-i}$

-


**Rationality requirement:** rational individuals will not use strictly dominated strategies.

**Procedure of iteratively deleting dominated strategies:** 

1. Mark all dominated strategies for all players, then delete all marked strategies
2. Apply step 1 to the resulting game
3. Continue this process until a game without dominated strategies results.

A game is *dominance solvable* if after IDDS all players are indifferent between all strategies that have survived.

Necessary assumption: **common knowledge** of rationality of all players, i.e. all players know that all players know that ... all players are rational.

Results after elimination of weakly dominated strategies can depend on order and number of strategies that are deleted.

--
A strategy profile $s^*$ constitutes a **Nash equilibrium** of the game $\Gamma_N$ if for every $i$, $$u_i(s_1^*, ..., s_i^*, ...,s_n^*)\ge u_i(s_1^*, ..., s_i, ...,s_n^*)$$ for all $s_i\in S_i$.

--

That is, $s_i^*$ is a best response to $s_{-i}$ for all $i$.

The **best response correspondence** is the correspondence $b_i(s_{-i})$ that maximizes the payoffs of player $i$ for each strategy of the other players.

-
A strategy profile $s$ is a Nash equilibrium of the normal form game $\Gamma_N$ is for all $i$ we have $s_i\in b(s_{-i})$

-

How to find a Nash equilibrium of a normal form game:

* Determine best responses/reaction functions (with FOCs) and determine intersections
* Trial and error (Bertrand)
* Guess an equilibrium and confirm. Check for uniqueness

-
If the strategies $(s_1^*, ..., s_I^*)$ are a Nash equilibrium, then they survive iterated elimination of strictly dominated strategies. 

-
-
If only the strategies $(s_1, ..., s_I^*)$ survive iterated elimination of strictly dominated strategies then these strategies are the unique Nash equilibrium of the normal form game $(\ \Gamma_N)$

-

-
Given a player $i$'s pure strategy set $S_i$, a *mixed strategy* $\sigma_i$ assigns to each pure strategy $s_i\in S_i$ a probability $\sigma_i(s_i)\ge 0$ that it will be played with.

-

A mixed strategy profile $\sigma^*=(\sigma_1^,...,\sigma_I^*)$ constitutes a Nash equilibrium of game $\Gamma_N$ if for every $i$,
$$u_i(\sigma_i^*,\sigma_{-i}^*)\ge u_i(\sigma_i',\sigma_{-i}^*) \text{ for all }\sigma_i'\in (S_i)$$


