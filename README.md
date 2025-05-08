# research-on-renminbi-exchange-rate-forecast
**研究正在进行阶段，代码及相关数据持续更新...**

**写在前面：**
  
  1. 由简入难逐步改进人民币汇率预测模型，基准模型考虑LSTM/XGboost/DLinear，只考虑输入汇率的时间序列数据。
  2. 计划的改进方向包括：利用信号处理技术如EMD、小波分解等对汇率数据进行预处理；将宏观数据如美元指数、GDP等数据融入输入端；考虑集成学习的方法融合基准模型。
  3. **References** The code about LSTM&DLinear is inspired by [EmmaHLU
ExchangeRateForecasting](https://github.com/EmmaHLU/ExchangeRateForecasting)

**目前进度：**
1. 现有文章存在的问题是大多数添加的指标都很少，而且几乎都是一次性经验模态分解（存在信息泄露问题），实际应用价值有限。
	a.   通过动态对冲的方式初步解决了该问题，现有模型框架如下![基于动态CEEMDAN-LSTM的汇率预测框架图](https://github.com/user-attachments/assets/32a213a6-4460-4a23-9241-0f01d7e32369)
	b.   现有代码见“动态CEEMDAN-LSTM.ipynb”
3. 后续计划尝试在经验模态分解方法处入手解决问题......

