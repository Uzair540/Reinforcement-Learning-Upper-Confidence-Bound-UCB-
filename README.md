# Reinforcement Learning Upper Confidence Bound UCB
## Implementing Machine Learning Algorithm : Reinforcement Learning Upper Confidence Bound (UCB) on the data-set of Ads CTR Optimization
### Upper Confidence Bound (UCB)
#### The multi-armed Bandit Problem
Trying to find the optimal option among many possible options as quickly as possible, with minimal exploration of other options which have high disadvantage in money (resources) and time. For example, if an Advertising company has 5 advertisement options, they need to find the best one to publish. In order to do this, they might to AB testing. But if they do too much AB testing, then it is just as same as utilizing all 5 options which is not ideal. Therefore, through reinforcement learning, the company needs to find the optimal option quickly.

The algorithm starts with an initial expecte value. Then, select a column and exploit it one time. The expected value might go down or up as new observation is taken. As there are more observations, the confidence bound gets smaller as the algorithm is more confident in the result. Then, select the column with the hiest upper confidence bound and exploit it once, which also makes the bound gets smaller and shifts the observation. Repeat these steps until the algorithm consistently exploits the same column, which is an indicator that this column is the optimal model.

This is different from simple Supervised Learning, as this model starts with no data. When we start experimenting to collect data, reinforcement learning determines what to do with that existing data
