# GC_24_IE801_ReinforcementLearning

## Baseline: stable-baselines3
- Documentation: https://stable-baselines3.readthedocs.io/en/master/guide/install.html
- Github: https://github.com/DLR-RM/stable-baselines3/tree/master
- Install with development version
	- git clone https://github.com/DLR-RM/stable-baselines3 && cd stable-baselines3
	- pip install -e .[docs,tests,extra]
- Run example 1: https://stable-baselines3.readthedocs.io/en/master/guide/examples.html
- Run example 2: https://rl-baselines3-zoo.readthedocs.io/en/master/
	- git clone https://github.com/DLR-RM/rl-baselines3-zoo
	- cd rl-baselines3-zoo/
	- pip install –e .
	- python train.py --algo dqn --env LunarLander-v3 -n 30000 --eval-episodes 10 --eval-freq 10000 --save-freq 10000
	- copy ./logs/dqn folder to /rl-trained-agents/.
	- python3 scripts/all_plots.py -a dqn --env LunarLander-v3 -f rl-trained-agents/

## Reference
[Solving the Lunar Lander Problem with Multiple Uncertainties using a Deep Q-Learning based Short-Term Memory Agent]
- https://dl.acm.org/doi/abs/10.1145/3633637.3633641

[DQN with model-based exploration: efficient learning on environments with sparse rewards]
- https://arxiv.org/abs/1903.09295
- https://github.com/stephengou/Deep-Q-Learning-with-Model-Based-Exploration

[Averaged-DQN: Variance Reduction and Stabilization for Deep Reinforcement Learning]
- https://proceedings.mlr.press/v70/anschel17a.html
- https://github.com/YiSyuanChen/Averaged-DQN

[Safety and Liveness Guarantees through Reach-Avoid Reinforcement Learning]
- https://www.roboticsproceedings.org/rss17/p077.pdf


