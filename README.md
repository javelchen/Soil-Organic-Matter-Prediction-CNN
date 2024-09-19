# Soil Organic Matter Prediction Model

## 项目简介
本项目旨在使用光谱数据和环境变量预测土壤有机质（SOM）含量。通过构建一个一维卷积神经网络（1D-CNN），结合光谱数据、时间相关矩阵（TDCS）和海拔信息，以提高SOC的预测精度。

## 目录
- [安装](#安装)
- [数据集](#数据集)
- [使用方法](#使用方法)
- [模型架构](#模型架构)
- [结果与评估](#结果与评估)
- [贡献](#贡献)
- [许可证](#许可证)

## 安装
确保你的环境中已安装以下软件和库：
- Python 3.x
- Jupyter Notebook（可选）
- NumPy
- Pandas
- SciPy
- scikit-learn
- Matplotlib
- TensorFlow

可以使用以下命令安装所需的库：
```bash
pip install numpy pandas scipy scikit-learn matplotlib tensorflow

## 数据集
- `mergedUK_OCdata.csv`: 包含光谱数据和对应的土壤有机质（SOM）值。
- `elevation.ipynb`: 包含海拔数据的Jupyter Notebook。

## 使用方法
1. 下载或克隆该仓库：
git clone https://github.com/javelchen/Soil-Organic-Matter-Prediction-CNN.git cd Soil-Organic-Matter-Prediction-CNN
2. 在 Jupyter Notebook 或 Python 脚本中运行 `soil_prediction.py` 或 `soil_prediction_model.ipynb` 文件。

3. 根据需要修改参数和配置，以适应你的数据。

## 模型架构
本模型使用一维卷积神经网络（1D-CNN），具体架构如下：
- 输入层：光谱数据和TDCS矩阵。
- 第1卷积层：32个滤波器，3x1核大小，ReLU激活函数。
- 第2卷积层：64个滤波器，3x1核大小，ReLU激活函数。
- 第3卷积层：64个滤波器，3x1核大小，ReLU激活函数。
- 最大池化层：降低维度。
- 全连接层：64个神经元，ReLU激活函数。
- 输出层：回归输出，预测SOM值。

## 结果与评估
模型的性能通过均方误差（MSE）和决定系数（R²）进行评估。训练完成后，可以查看模型的预测效果，并通过可视化手段展示实际值与预测值之间的关系。

## 贡献
欢迎任何形式的贡献！如果你有想法或建议，请提交问题或拉取请求。

## 许可证
本项目遵循 [MIT 许可证](LICENSE)。
