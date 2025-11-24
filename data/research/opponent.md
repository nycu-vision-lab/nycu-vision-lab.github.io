## Opponent Exploitation

In a multi-agent competitive environment, it is important for an agent to detect the
opponent’s policy and adopt a suitable policy to exploit the opponent. Conventionally,
most methods, e.g., Bayesian policy reuse (BPR) variants, assume that the opponent
adopts a fixed policy or a randomly changing policy.

In this work, we make a more realistic assumption that the opponent may select its
policy based on previous observations. We define a “strategy” as the mapping from the
previous observation to the opponent’s selected policy, and propose a Bayesian strategy
inference (BSI) framework to infer the opponent’s strategy. Furthermore, to deal with
opponents who may randomly select their policies, the BSI framework is combined with an
intra-episode policy tracking mechanism to construct the Bayesian strategy inference
plus policy tracking (BSI-PT) algorithm.

Experiments on an Extended Batter versus Pitcher game (EBvPG) show that BSI-PT
achieves higher policy prediction accuracy and winning percentage than three other BPR
variants against opponents with fixed, random, or partially random policy selection
strategies.

<span class="muted">
Reference: Lee, Kuei-Tso, et al., “Opponent exploitation based on bayesian strategy
inference and policy tracking,” <em>IEEE Transactions on Games</em>, Vol.16, No.2, June 2024.
</span>
