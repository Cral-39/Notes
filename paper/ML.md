# 《_IoTJ__Parameterized_DRL_for_Computation_Offloading___Major》
## 一. 预备知识

#### 1.机器学习基础
##### （1）机器学习类型：
+ Supervised learning（监督学习）
+ Unsupervised learning（无监督学习）
##### （2）监督学习：学习从输入到输出的映射。关键特征：给学习算法提供包含正确答案的实例
+ Regression algorithms（回归算法）：Predict a number infiitely many possible outputs
+ classification algorithms（分类算法）：Predict categories small number of possible outputs
##### (3)无监督学习：Data only comes with inputs x，but not output labels y.Algorithrm has to find **structure** in the data
+ Clustering（聚类算法）：处理无标签数据并尝试自动将他们分组进簇中
+ Anomalt detection（异常检测）：用于检测异常事件
+ Dimensionality reduction（降维）：Compress data using fewer numbers
##### （4）Linear regression线性回归模型（一种监督学习模型）
  +  traning set（训练集）：用于训练模型的数据集
  +  x="input"variable/feature
  +  y="output"variable/"target"variable
  +  m=number of training examples
  +  (x,y)=single training example
  +  y-hat：y的估计值或预测值
##### （3）测试：评估训练好的模型在新数据上表现如何的过程。
+ Note：泛化性**Generalizability**即举一反三能力
### 2.初步学习（大模型给出）
##### 多接入边缘计算（MEC）
+ 多接入边缘计算（Multi-access Edge Computing，简称 MEC）是一种将计算、存储和网络服务下沉到网络边缘（如基站、接入点或边缘数据中心）的技术架构。其核心目标是通过将云服务从远程数据中心“拉近”到用户附近，降低延迟、节省带宽、提升用户体验，并支持实时性要求高的应用（如AR/VR、自动驾驶、工业物联网等）。
##### 任务卸载策略
+ 任务卸载策略就是“在动态环境、有限资源、多重约束下，用算法实时决定任务该在哪执行”，让端-边-云协同达到更快、更省、更稳的平衡。
##### 深度强化学习（DRL）
+ 深度强化学习（Deep Reinforcement Learning, DRL）= 强化学习（试错、奖励）+ 深度神经网络（高维表征）。
核心思路：
把“状态→动作”的决策函数（策略）或“状态→价值”的估值函数用深度网络来近似，端到端地直接输入像素、语音、传感器等高维原始数据，用奖励信号反向传播更新网络，使智能体在环境中自我试错、持续改进。
