

# 一、赛题背景

糖尿病是全球最普遍的慢性疾病之一，每年影响数全球千万人，给经济带来沉重的经济负担。糖尿病对人体的健康危害也不容小嘘，个人失去有效调节血液中葡萄糖水平的能力，需要长期药物干预治疗，并可能导致生活质量和预期寿命下降。

在消化过程中，不同的食物被分解成糖后，糖就会被释放到血液中。这向胰腺发出释放胰岛素的信号。胰岛素有助于体内的细胞利用血液中的这些糖来获取能量。糖尿病通常的特点是身体没有产生足够的胰岛素，或者无法根据需要有效地使用胰岛素。

# 二、赛事任务

本次比赛任务是根据健康指标相关信息数据，然后通过训练数据训练模型，预测测试集所属类别。目标分为三类，0为非糖尿病，1为糖尿病前期，2为糖尿病。

# 三、使用

代码写的比较乱

代码中，做了一些**EDA**，可以不使用这里面的代码

**特征工程**

做了很多特征，具体看代码，但是都没有上分，这是很不应该的

**另外发现**：很多不应该出现的小数，所有列都有这种情况，如性别，只可能是0和1，但是经过EDA却发现了很多0.几的情况，

利用四舍五入进行处理，将所有列变成整数，经过训练检测结果反而不好，原因不清楚，不符合基本认知，推测是过拟合了

上分主要是用lgb，和smote过采样，因为发现样本不均衡，

**里面的特征工程的构造思想，归一化操作，过采样方法，以及多分类模型后续都可以被其他任务使用，作为积累**
