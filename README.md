# youtube-viral-video-analysis
YouTube Viral Video Analysis and Popular Content Prediction
# YouTube爆款视频形成机制分析与热门内容预测

## 项目简介

本项目基于 YouTube Trending 数据集，通过数据分析与机器学习方法，探索影响视频成为爆款的关键因素，并构建热门内容预测模型。

项目从内容属性、发布时间、创作者影响力等多个维度展开分析，结合探索性数据分析（EDA）、SQL指标构建以及机器学习建模，形成从业务问题提出到预测模型落地的完整分析闭环。

---

## 项目背景

随着内容平台竞争日益激烈，如何识别潜在爆款内容、优化内容运营策略以及提高流量分发效率，已成为平台和创作者关注的重要问题。

本项目围绕以下业务问题展开分析：

- 哪些内容分类更容易产生爆款视频？
- 发布时间是否会影响视频传播效果？
- 创作者影响力是否决定视频热度表现？
- 内容包装因素是否会影响传播效果？
- 能否利用机器学习预测视频是否会成为爆款？

---

## 项目分析框架

<img width="1215" height="1295" alt="image" src="https://github.com/user-attachments/assets/8c6253b9-7a9b-4f86-b409-afd68ed9f0f6" />


---

## 数据来源

**数据集：** YouTube Trending Dataset

**研究对象：** 美国地区 Trending 榜单视频

**样本规模：** 6,351 条去重后的视频记录

**主要字段：**

- 视频标题（title）
- 视频分类（category_name）
- 发布时间（publish_time）
- 播放量（views）
- 点赞量（likes）
- 评论量（comment_count）
- 标签信息（tags）
- 频道信息（channel_title）

---

## 技术栈

### 数据处理

- Python
- Pandas
- NumPy

### 数据分析

- SQL
- Matplotlib
- Seaborn

### 机器学习

- Scikit-Learn
- XGBoost

---

## 项目内容

### 1. 数据清洗与特征工程

- 缺失值处理
- 重复视频去重
- 时间特征提取
- 创作者影响力指标构建
- 爆款标签构建

### 2. 探索性数据分析（EDA）

- 内容生态分析
- 视频分类分析
- 创作者分析
- 用户互动分析

### 3. 爆款形成机制分析

从以下维度分析爆款形成规律：

- 内容赛道
- 创作者影响力
- 发布时间
- 内容包装

### 4. 爆款预测模型构建

构建并比较三类模型：

- Logistic Regression
- Random Forest
- XGBoost

评估指标：

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC

---

## 核心发现

### 创作者影响力是爆款形成的核心因素

特征重要性分析结果显示，创作者影响力相关指标对爆款预测贡献最大。

### 内容赛道存在明显传播差异

Music、Entertainment 等类别整体表现优于其他内容类别。

### 发布时间会影响传播效果

发布时间相关特征具备一定预测能力，合理安排发布时间有助于提高内容曝光机会。

### 机器学习能够有效识别潜在爆款

Random Forest 在三类模型中表现最佳，验证了利用公开视频数据预测热门内容的可行性。

---

## 项目价值

本项目完成了从业务问题提出、数据分析、规律验证到机器学习预测的完整分析流程。

研究结果表明，即使在缺少平台内部用户行为数据（CTR、完播率、观看时长等）的情况下，仍能够利用公开数据识别影响内容传播的重要因素，为内容运营、创作者成长分析以及热门内容预测提供数据支持。

---

## 项目结构

```text
youtube-viral-video-analysis
│
├── README.md
├── framework.png
├── youtube_analysis.ipynb
├── youtube_analysis.html
└── YouTube爆款视频形成机制分析与热门内容预测.pdf
```

---

## 项目成果展示

### 核心结论

> 创作者影响力 ＞ 内容赛道 ＞ 发布时间 ＞ 内容包装

### 最优模型

- Model：Random Forest
- Evaluation：Accuracy、Precision、Recall、F1 Score、ROC-AUC 综合表现最佳

### 应用价值

- 热门内容识别
- 内容运营优化
- 创作者成长分析
- 爆款内容预测

---

## 作者：程银龙

如对项目内容感兴趣，欢迎交流讨论。
