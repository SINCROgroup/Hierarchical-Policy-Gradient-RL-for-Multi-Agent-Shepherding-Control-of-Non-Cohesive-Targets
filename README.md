# Hierarchical-Policy-Gradient-RL-for-Multi-Agent-Shepherding-Control-of-Non-Cohesive-Targets

*Abstract: We propose a decentralized reinforcement learning solution for multi-agent shepherding of non-cohesive targets using policy-gradient methods. Our architecture integrates target-selection with target-driving through Proximal Policy Optimization, overcoming discrete-action constraints of previous Deep Q-Network approaches and enabling smoother agent trajectories. This model-free framework effectively solves the shepherding problem without prior dynamics knowledge. Experiments demonstrate our method’s effectiveness and scalability with increased target numbers and limited sensing capabilities.*

This repository contains the numerical simulations discussed in 
```
@ARTICLE{arXiv:2504.02479,
  author={Stefano, Covone and Italo, Napolitano and De Lellis, Francesco and di Bernardo, Mario},
  journal={arXiv:2504.02479, 
  title={Hierarchical Policy-Gradient Reinforcement Learning for Multi-Agent Shepherding Control of Non-Cohesive Targets}, 
  year={2025}}
```
In this context, a group of herder agents works to corral and contain a group of target agents within a goal region in the plane.

Folder organization:

- "N_1_M_1.mp4": This video corresponds to the simulation in Section IV.A, shown in Figure 3 in [1]. A single herder (blue diamond) corrals and contains a single target (magenta dot) within the goal region (black circle), successfully completing the task.
  
- "N_2_M_5.mp4": This video illustrates the example discussed in Section V.A of [1], shown in Figure 4. Here, two herders (blue diamonds) corral and contain five targets (magenta dots) within the goal region (black circle).

- "N_10_M_100.mp4": This video shows the simulation discussed in Section V.C and depicted in Figure 6 of [1]. The previously trained network, designed for a two-herder, five-target scenario, is extended to handle 10 herders and 100 targets. Each herder is limited to sensing the five closest targets and the nearest herder, demonstrating the scalability and effectiveness of the proposed solution.

[1]: Stefano Covone, Italo Napolitano, Francesco De Lellis, Mario di Bernardo, "Hierarchical Policy-Gradient Reinforcement Learning for Multi-Agent Shepherding Control of Non-Cohesive Targets," submitted for pubblication in the proceedings of, and presentation at the Conference on Decision and Control 2025.
