# 🚀 Credit Risk Scoring AI

## 📌 项目简介
本项目旨在构建一个 **信用评分模型**，用于预测用户的违约风险。我们结合 **SQL 数据操作、机器学习模型对比、数据可视化**，打造一个完整的信用风险分析系统。

### **核心功能**
- **数据获取与存储**：使用 SQL 提取、清理并处理数据。
- **数据探索与可视化**：分析信用评分、收入、贷款金额等关键特征。
- **特征工程**：创建信用风险相关的新特征，如收入与贷款比率。
- **机器学习模型训练**：比较 **Logistic Regression、XGBoost、LightGBM** 等模型。
- **模型评估**：使用 AUC、准确率等指标评估模型性能。
- **结果可视化**：绘制数据分布图、模型对比图，提高可解释性。

---

## 📂 目录结构
本项目按照模块化结构设计，方便扩展与维护。
```
credit-risk-scoring/
│── data/                     # 数据存放（不直接上传）
│   ├── raw_data.csv          # 原始 CSV 数据
│   ├── processed_data.csv     # 预处理后的数据
│
│── notebooks/                 # Jupyter Notebook 存放
│   ├── EDA.ipynb              # 数据探索 & 可视化
│   ├── Feature_Engineering.ipynb # 特征工程 & SQL 处理
│   ├── Model_Comparison.ipynb # 机器学习模型对比
│
│── sql/                      # SQL 脚本存放
│   ├── data_extraction.sql    # 数据提取 SQL 语句
│   ├── data_cleaning.sql      # 数据清洗 SQL 语句
│
│── src/                      # Python 代码
│   ├── data_loader.py        # 读取 SQL 数据
│   ├── feature_engineering.py # 特征工程
│   ├── model_training.py      # 训练多个模型
│   ├── visualization.py       # 结果可视化
│
│── results/                   # 结果存放
│   ├── model_performance.png  # 模型对比图
│
│── README.md                  # 项目说明
│── requirements.txt           # 依赖包
│── LICENSE                    # 开源许可
```

---

## 🔧 **项目步骤**
本项目按照以下步骤进行：

### **1️⃣ 数据获取与存储**
- 选择合适的数据集，如 **Kaggle Home Credit Default Risk**。
- 使用 SQL 进行数据提取、清洗，并存入数据库。
- 通过 Pandas 读取数据库数据，进行基本数据探索。

### **2️⃣ 数据探索（EDA）**
- 统计数据特征，如信用评分分布、收入情况等。
- 处理缺失值、异常值，确保数据质量。
- 绘制相关性矩阵，分析特征间的关系。

### **3️⃣ 特征工程**
- 创建新的信用风险特征，如 **收入/贷款比率、年龄分组等**。
- 进行特征缩放、类别变量处理，提高模型泛化能力。
- 使用 SQL + Pandas 进行特征生成。

### **4️⃣ 机器学习模型训练**
- 选择 **Logistic Regression、XGBoost、LightGBM** 进行建模。
- 采用交叉验证方式，确保模型稳健性。
- 计算 AUC、准确率等关键指标，评估模型效果。

### **5️⃣ 结果可视化**
- 绘制数据分布图，如信用评分直方图。
- 生成模型表现对比图，展示 AUC、准确率。
- 通过 SHAP 解释模型，分析重要特征。

### **6️⃣ 运行与部署**
- 通过 `requirements.txt` 安装依赖。
- 运行 SQL 脚本，准备数据库。
- 运行模型训练脚本，生成信用评分预测。

---

## 🚀 **如何运行本项目？**
### **1️⃣ 安装依赖**
```sh
pip install -r requirements.txt
```

### **2️⃣ 运行 SQL 脚本 & 加载数据**
```sh
sqlite3 database.db < sql/data_extraction.sql
```

### **3️⃣ 训练模型**
```sh
python src/model_training.py
```

### **4️⃣ 生成可视化结果**
```sh
python src/visualization.py
```

---

## 📜 **许可证**
本项目基于 **MIT License** 开源。欢迎贡献和改进！

