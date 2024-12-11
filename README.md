# GC_24_IE801_ReinforcementLearning

## Baseline: stable-baselines3
- Documentation 1: https://stable-baselines3.readthedocs.io/en/master/guide/install.html
- Documentation 2: https://rl-baselines3-zoo.readthedocs.io/en/master/
- Github 1: https://github.com/DLR-RM/stable-baselines3/tree/master
- Github 2: https://github.com/DLR-RM/rl-baselines3-zoo?tab=readme-ov-file
- Install with development version
	- git clone https://github.com/DLR-RM/stable-baselines3 && cd stable-baselines3
	- pip install -e .[docs,tests,extra]
- Run:
	- git clone https://github.com/DLR-RM/rl-baselines3-zoo
	- cd rl-baselines3-zoo/
	- pip install –e .
	- python train.py --algo dqn --env LunarLander-v3(or MountainCar-v0)
- Plot:
	- python scripts/all_plots.py -a dqn --env LunarLander-v3(or MountainCar-v0) -f rl-trained-agents/directory_name_which_is_copied_from_rl-baselines3-zoo/logs
- Record:
	- python -m rl_zoo3.record_video --algo dqn --env LunarLander-v3(or MountainCar-v0) -n 1000 --load-best -f rl-trained-agents/directory_name_which_is_copied_from_rl-baselines3-zoo/logs

## Reference
- Lunar Lander v3 (https://gymnasium.farama.org/environments/box2d/lunar_lander/)
- Mountain Car v0 (https://gymnasium.farama.org/environments/classic_control/mountain_car/)
- Human-level control through deep reinforcement learning (https://www.nature.com/articles/nature14236)
- Averaged-DQN: Variance Reduction and Stabilization for Deep Reinforcement Learning (https://proceedings.mlr.press/v70/anschel17a.html)(code: https://github.com/stephengou/Deep-Q-Learning-with-Model-Based-Exploration)
- DQN with model-based exploration: efficient learning on environments with sparse rewards (https://arxiv.org/abs/1903.09295)(code: https://github.com/stephengou/Deep-Q-Learning-with-Model-Based-Exploration)
- Solving the Lunar Lander Problem with Multiple Uncertainties using a Deep Q-Learning based Short-Term Memory Agent (https://dl.acm.org/doi/fullHtml/10.1145/3633637.3633641)
- Safety and Liveness Guarantees through Reach-Avoid Reinforcement Learning (https://www.roboticsproceedings.org/rss17/p077.pdf)
