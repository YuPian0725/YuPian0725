# 蘑菇数据集🍄
气味是野外识别蘑菇安全性的最直观感官指标。通过生成饼图、环形图、直方图、热力图等专业图形，对蘑菇数据集进行可视化分析。旨在研究**蘑菇的气味与毒性之间的相关性**
# 数据来源
本报告使用的数据集为UCI Machine Learning Repository提供的经典Mushroom Dataset （蘑菇数据集）<br>
### 数据获取方式
通过UCI机器学习库官方网站公开下载
# 数据集的基本情况
数据集包含8124个蘑菇样本。每个样本由23个属性描述。所有属性均为离散型名义变量。<br>
数据集的类别标签将蘑菇分为两类：**可使用（Edible）** 和 **不可食用（Poisonous）** <br>
22个特征变量涵盖蘑菇的物理外观和生长环境 <br>
* 菌盖特征：菌盖形状（cap-shape）、菌盖表面（cap-surface）、菌盖颜色（cap-color）<br>
* 菌褶特征：菌褶附着方式（gill-attachment）、菌褶间距（gill-spacing）、菌褶大小（gill-size）、菌褶颜色（gill-color）<br>
* 菌柄特征：菌柄形状（stalk-shape）、菌柄根部（stalk-root）、菌柄表面（stalk-surface）<br>
* 其他特征：气味（odor）、是否有瘀伤（bruises）、孢子印颜色（spore-print-color）<br>
* 生长环境：种群分布（population）、栖息地（habitat）<br>
# 数据预处理与清理
1.加载与检查数据<br>
2.缺失值处理<br>
* 查找缺失值<br>
* 填充缺失值<br>

3.属性值映射<br>
4.对气味(odor)进行映射：<br>
* a--Almond（杏仁味）<br>
* l--Anise（茴香味）<br>
* c--Creosote（杂酚油味）<br>
* y--Fishy（鱼腥味）<br>
* f--Foul（恶臭味）<br>
* m--Musty（霉味）<br>
* n--None（无味）<br>
* p--Pungent（辛辣味）<br>
* s--Spicy（香料味）<br>

类别标签e/p分别映射为Edible（可食用）/Poisonous（有毒）
5.清理后数据最终形态
8124行样本*23列变量，所有特征变量保持完整，stalk-root增加"unknown"类别。核心变量odor（9个类别）和class（2个类别）均无缺失
# 可视化
气味--毒性之间的相关性（饼图，柱形图，直方图，热力图）
