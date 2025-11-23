# 这里是我用来记录自己学习机器学习的项目

## 机器学习简介

机器学习是一种通过数据和经验来改进计算机性能的技术。它涉及算法和统计模型，使计算机系统能够自动从数据中学习和做出预测或决策，而无需明确编程。

## 项目结构

- `datasets/`：存放数据集的文件夹。
- `machine_learning/`：包含各个传统机器学习算法的详细程序，使用ipynb文件编写。
- `deep_learning/`：包含深度学习相关的程序和模型，使用ipynb文件编写。

## 机器学习分类

| 学习类型   | 解释                                                                                     |
| ---------- | ---------------------------------------------------------------------------------------- |
| 监督学习   | 如果我们的数据集是**有标签**的，那么我们把这种**学习任务**叫做监督学习。     |
| 无监督学习 | 如果我们的数据集是**没有标签**的，那么我们把这种学习任务叫做**无监督学习**。 |
| 强化学习   | 这种学习任务是通过**智能体与环境**的交互来进行学习的一种学习任务。                 |

```mermaid
flowchart TD
    %% 四大核心机器学习板块
    A[机器学习] --> B[监督学习]
    A --> C[无监督学习]
    A --> D[强化学习]
  
    %% 深度学习作为技术基础
    E[深度学习<br>核心技术] --> B
    E --> C
    E --> D
  
    %% 监督学习的子任务
    B --> F[主要任务]
    F --> G[分类<br>预测离散类别]
    F --> H[回归<br>预测连续数值]
  
    %% 无监督学习的子任务
    C --> I[主要任务]
    I --> J[聚类<br>数据分组]
    I --> K[降维<br>特征简化]
    I --> L[关联规则<br>发现关系]
  
    %% 强化学习的核心概念
    D --> M[核心机制]
    M --> N[智能体-环境交互]
    M --> O[奖励信号驱动]
    M --> P[策略学习]
  
    %% 优化样式 - 简洁清晰的配色
    style A fill:#2E86AB,stroke:#333,stroke-width:3px,color:#fff,font-weight:bold
    style E fill:#A23B72,stroke:#333,stroke-width:2px,color:#fff,font-weight:bold
    style B fill:#F18F01,stroke:#333,color:#000
    style C fill:#C73E1D,stroke:#333,color:#fff
    style D fill:#3BB273,stroke:#333,color:#000
  
    style F fill:#F18F01,stroke:#333,color:#000
    style G fill:#F18F01,stroke:#333,color:#000
    style H fill:#F18F01,stroke:#333,color:#000
  
    style I fill:#C73E1D,stroke:#333,color:#fff
    style J fill:#C73E1D,stroke:#333,color:#fff
    style K fill:#C73E1D,stroke:#333,color:#fff
    style L fill:#C73E1D,stroke:#333,color:#fff
  
    style M fill:#3BB273,stroke:#333,color:#000
    style N fill:#3BB273,stroke:#333,color:#000
    style O fill:#3BB273,stroke:#333,color:#000
    style P fill:#3BB273,stroke:#333,color:#000
```
# 各种学习之间的关系
```mermaid
flowchart TD
    subgraph C [高级学习范式]
        direction LR
        D[迁移学习<br>解决“数据/算力少”]
        E[元学习<br>解决“学得慢”]
    end

    subgraph B [核心技术]
        F[深度学习<br>神经网络等]
    end

    subgraph A [基础学习范式]
        direction LR
        G[监督学习]
        H[无监督学习]
        I[强化学习]
    end

    C --> B --> A
```