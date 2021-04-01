# PN-Diode-Potential-Prediction
该项目复现了Dr. S.M-Hong在2019SISPAD的论文： Han, Seung-Cheol, and Sung-Min Hong. "Deep neural network for generation of the initial electrostatic potential profile." 2019 International Conference on Simulation of Semiconductor Processes and Devices (SISPAD). IEEE, 2019.

【数据集获得】在Global TCAD Solution软件中，求解Non-Lineae Poisson方程，得到了一个PN结内建电势分布。改变PN结内载流子掺杂，得到1156个样本。特征是P区和N区的Doping Concentration，特征是pn结内121处的势能分布。

【训练及测试】随机1：1划分train set和test set。Epoch 1000, LR=1e-5。基本上可以很好的拟合PN结内势能分布。
