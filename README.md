# 🚀 Credit Risk Scoring AI | 信用评分 AI

## 📌 Project Overview | 项目简介
This project aims to build a **Credit Risk Scoring Model** to predict user default risk.

- **Data Handling**: Use SQL to extract, clean, and process data.
- **Model Comparison**: Train and evaluate **Logistic Regression, XGBoost, LightGBM**.
- **Visualization**: Analyze data distribution, feature importance, and model performance.
- **GitHub Representation**: Include SQL queries, feature engineering, and Jupyter Notebook examples.

本项目旨在构建一个 **信用评分模型**，用于预测用户的违约风险。

- **数据获取与存储**：使用 SQL 提取、清理并处理数据。
- **模型对比**：使用 **Logistic Regression, XGBoost, LightGBM** 进行训练。
- **可视化**：分析数据分布、特征重要性，并展示模型对比结果。
- **GitHub 体现**：提供 SQL 查询、特征工程、训练代码，并包含 Jupyter Notebook 示例。

---

## 📂 Directory Structure | 目录结构
```
credit-risk-scoring/
│── data/                     # Data storage (local) | 数据存放（本地）
│   ├── raw_data.csv          # Raw CSV data | 原始 CSV 数据
│   ├── processed_data.csv     # Processed data | 预处理后的数据
│
│── notebooks/                 # Jupyter Notebooks
│   ├── EDA.ipynb              # Data Exploration & Visualization | 数据探索 & 可视化
│   ├── Feature_Engineering.ipynb # Feature Engineering & SQL Processing | 特征工程 & SQL 处理
│   ├── Model_Comparison.ipynb # Model Comparison | 机器学习模型对比
│
│── sql/                      # SQL Scripts | SQL 脚本
│   ├── data_extraction.sql    # Data Extraction SQL | 数据提取 SQL 语句
│   ├── data_cleaning.sql      # Data Cleaning SQL | 数据清洗 SQL 语句
│
│── src/                      # Python Scripts | Python 代码
│   ├── data_loader.py        # SQL Data Loader | 读取 SQL 数据
│   ├── feature_engineering.py # Feature Engineering | 特征工程
│   ├── model_training.py      # Model Training | 训练多个模型
│   ├── visualization.py       # Results Visualization | 结果可视化
│
│── results/                   # Results Storage | 结果存放
│   ├── model_performance.png  # Model Performance Visualization | 模型对比图
│
│── README.md                  # Project Documentation | 项目说明
│── requirements.txt           # Dependencies | 依赖包
│── LICENSE                    # Open Source License | 开源许可
```

---

## 🔧 Project Steps | 项目步骤
This project follows these key steps:

本项目按照以下步骤进行：

### **1️⃣ Data Extraction & Storage | 数据获取与存储**
- Select an appropriate dataset, such as **Kaggle Home Credit Default Risk**.
- Use SQL to extract, clean, and store the data.
- Read database data using Pandas for basic exploration.

- 选择合适的数据集，如 **Kaggle Home Credit Default Risk**。
- 使用 SQL 进行数据提取、清理，并存入数据库。
- 通过 Pandas 读取数据库数据，进行基本数据探索。

### **2️⃣ Exploratory Data Analysis (EDA) | 数据探索**
- Analyze statistical characteristics such as credit score distribution.
- Handle missing values and outliers.
- Visualize feature relationships using correlation matrices.

- 统计数据特征，如信用评分分布、收入情况等。
- 处理缺失值、异常值，确保数据质量。
- 绘制相关性矩阵，分析特征间的关系。

### **3️⃣ Feature Engineering | 特征工程**
- Create new credit risk features such as **income-to-loan ratio, age groups**.
- Perform feature scaling and categorical encoding.
- Generate features using SQL + Pandas.

- 创建新的信用风险特征，如 **收入/贷款比率、年龄分组等**。
- 进行特征缩放、类别变量处理，提高模型泛化能力。
- 使用 SQL + Pandas 进行特征生成。

### **4️⃣ Model Training | 机器学习模型训练**
- Train **Logistic Regression, XGBoost, LightGBM** models.
- Use cross-validation to ensure model robustness.
- Compute key metrics such as AUC and accuracy.

- 选择 **Logistic Regression、XGBoost、LightGBM** 进行建模。
- 采用交叉验证方式，确保模型稳健性。
- 计算 AUC、准确率等关键指标，评估模型效果。

### **5️⃣ Model Evaluation & Visualization | 结果可视化**
- Plot data distributions, such as credit score histograms.
- Generate model performance comparison charts.
- Use SHAP analysis to interpret key features.

- 绘制数据分布图，如信用评分直方图。
- 生成模型表现对比图，展示 AUC、准确率。
- 通过 SHAP 解释模型，分析重要特征。

### **6️⃣ Running & Deployment | 运行与部署**
- Install dependencies from `requirements.txt`.
- Run SQL scripts to prepare the database.
- Execute the model training script to generate predictions.

- 通过 `requirements.txt` 安装依赖。
- 运行 SQL 脚本，准备数据库。
- 运行模型训练脚本，生成信用评分预测。

---

## 🚀 How to Run | 如何运行本项目？
### **1️⃣ Install Dependencies | 安装依赖**
```sh
pip install -r requirements.txt
```

### **2️⃣ Run SQL Scripts & Load Data | 运行 SQL 脚本 & 加载数据**
```sh
sqlite3 database.db < sql/data_extraction.sql
```

### **3️⃣ Train Models | 训练模型**
```sh
python src/model_training.py
```

### **4️⃣ Generate Visualization Results | 生成可视化结果**
```sh
python src/visualization.py
```

---

## 📜 License | 许可证
This project is open-source under the **MIT License**. Contributions are welcome!

本项目基于 **MIT License** 开源。欢迎贡献和改进！

