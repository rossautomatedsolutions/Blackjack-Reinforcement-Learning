# Teaching a Machine to Beat Blackjack: An RL Journey

Blackjack is one of the most widely studied games in both casinos and academia.  
The rules are simple, but the strategy is subtle, and the possibility of card counting has made it a fascinating testbed for probability, game theory, and decision-making.

This project explores a single question: **can a machine, using reinforcement learning (RL), teach itself how to play blackjack — and even rediscover professional strategies such as card counting?**

---

## Project Overview

The work is structured as a series of four Jupyter notebooks, each one building on the last:

### Notebook 1 – From Zero to Basic Strategy
- A toy blackjack environment with only two actions (**Hit/Stand**).  
- The agent starts with no knowledge and learns strategy from scratch using **Monte Carlo Control**.

### Notebook 2 – Scaling Up to Casino Blackjack
- Six-deck shoe with real casino rules (dealer stands on soft 17, blackjack pays 3:2).  
- **Double Down** added as an action.  
- **Q-learning** replaces Monte Carlo to handle the larger state/action space.

### Notebook 3 – Card Counting & Adaptive Betting
- Multi-deck shoe with penetration (shuffle only after 75% dealt).  
- A **card counting feature** is added to the state.  
- Variable **bet sizing actions** allow the agent to learn when to increase wagers.

### Notebook 4 – Deep RL for Blackjack
- Tabular methods give way to **function approximation**.  
- A **Deep Q-Network (DQN)** generalizes across the massive state/action space, combining play and betting decisions at scale.

---

## Results

Across the four stages, the agent progresses from:
- A naïve learner that discovers **basic strategy** through self-play.  
- To a **Q-learning agent** that adapts to real-world casino rules.  
- To a **card-counting system** that raises bets in favorable decks.  
- Finally, to a **deep RL model** capable of generalizing across thousands of states and actions.  

The learned strategies resemble professional blackjack heuristics, with play, doubling, and betting rules emerging naturally from experience.

---
