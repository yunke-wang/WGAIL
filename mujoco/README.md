# Learning to Weight Imperfect Demonstraitons (Experiment with Mujoco)
## Requirement
 * Python 3.7
 * torch 1.3.1
 * gym 0.15.7
 * mujoco 2.0.2.4
 * numpy 1.16.2
 
## Execute
 * w-GAIL
 ```
 python wgail.py --env Ant-v2 --num-epochs 5000 --traj-size 1000 --stage 2
 ```
 * 2IWIL
 ```
 python 2iwil.py --env Ant-v2 --num-epochs 5000 --traj-size 1000 --stage 2
 ```
 * GAIL
 ```
 python gail.py --env Ant-v2 --num-epochs 5000 --traj-size 1000 --stage 2
 ```
 * T-REX
 ```
 python trpo_irl.py --env Ant-v2 --num-epochs 5000 --reward-path 'reward_model/ant_reward_stage2.pth' --stage 2
 ```
