## 深度强化学习
###### 该笔记内容来自bilibili【王海森】深度强化学习课程

#### 一.基本概念
+ Random Variable（随机变量）X为随机变量，x为观测值
+ Probability Density Function（概率密度函数）：随机变量在某个确定的取值点附近的可能性
+ Expectation（期望）：
   <img src="屏幕截图 2025-09-26 214307.png">
+ Random Sampling（随机抽样）
+ state（状态）
+ Action（动作）
+ Agent（智能体）：动作的主体
+ policy ：根据agent的状态做出决策控制运动
+ reward：agent做出一个动作就给予奖励
+ state transitions（状态转移）
+ agent和environment的关系
<img src="屏幕截图 2025-09-26 215901.png">
+ 随机性的来源
   + actions的随机性：根据policy函数随机抽样得到
   + state transitions的随机性：环境跟状态转移函数p随机抽样

+ Return：未来的累计奖励
 + Discounted Return：折扣回报（未来的会有一定权重）
  <img src="屏幕截图 2025-09-26 232028.png">

 + Action-value function（动作价值函数）
 <img src="屏幕截图 2025-09-26 232615.png">

 + Optimal action-value function（最有动作价值函数）
<img src="屏幕截图 2025-09-26 232747.png">

 + State-value function（状态价值函数）
### 二.价值学习，Value-Based Reinforcement Learning
###### Deep Q-Network（DQN）：用神经网络来记住Q值
+ 使用TD算法来学习：TD（时序差分）算法用“当下立即奖励 + 下一刻估计值”来更新此刻估计值
<img src="屏幕截图 2025-09-26 231846.png">
