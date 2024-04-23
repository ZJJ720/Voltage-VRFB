# 全钒液流电池端电压模型

## 文件说明

文件 BiLSTM_ReLU.ipynb 在模型架构中引入 ReLU 激活函数
考虑了过去 30 个时间步的电压数据，以及当前时刻的温度、电流、SoC、SoH、流量数据，
预测未来 1 个时间步的电压数据。

文件 BiLTSM.ipynb 在模型架构中不引入 ReLU 激活函数
其余和 BiLSTM_ReLU.ipynb 一样

- BiLSTM_np_nd: 不引入 SoH 和过去电压数据

- BiLSTM_np:不引入过去电压数据

- BiLSTM / BiLSTM_ReLU:引入 SoH 和引入过去电压数据进行实验
