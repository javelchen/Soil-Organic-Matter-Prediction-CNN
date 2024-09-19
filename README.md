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
