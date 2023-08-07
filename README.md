# Deep_Embedd_Clustering
***Paper-Reproduce: (Proceedings of the CSEE) 基于深度嵌入聚类的水光荷不确定性源场景生成方法***

---

### File Information
1. **"2020年15分钟华东及四省一市的调度口径负荷.xlsx" "20191201至20201109华东及四省一市风光96点出力及装机容量.xlsx"** is the data.
2. **"基于深度嵌入聚类的水光荷不确定性源场景生成方法_杨晶显.pdf"** is the paper i reproduce.
3. **"深度嵌入聚类.ipynb"** is all the code.

### Methods Description
1. 随着水、光互补发电系统的应用越来越广泛，如何对水、光出力及负荷增长变化的不确定的融合特性建模对电网的运行调度及规划愈加重要。该文提出一种基于**深度嵌入聚类(DEC)**的水光荷不确定性源场景生成方法。
2. 利用**堆栈自编码(stacked auto-encoder，SAE)网络**提取水光荷不确定变量的初始特征，降低数据维度；
3. 利用 **KL(Kullback-Leibler)散度**优化聚类分配目标对自编码网络进行调整，采用**自适应矩估计(adaptive moment estimation，Adam)优化算法**得到模型最佳参数，通过对编码所嵌入的特征向量不断迭代优化，得到水光荷不确定性变量间的时空依赖关系，从而生成典型场景。
4. 算例分析以某地区电网实际采集数据为研究对象，利用**误差平方和(sum of squared error，SSE)、SIL、CHI** 指标对比传统聚类方法，验证了所提算法的有效性。实验结果如下所示：

![1](https://github.com/ArcherCYM/Deep_Embedd_Clustering/assets/49087999/7091d067-5f20-4758-82eb-e305ae813b83)

![2](https://github.com/ArcherCYM/Deep_Embedd_Clustering/assets/49087999/20c1c526-97cd-4de0-93a5-6af1eeac8297)

![3](https://github.com/ArcherCYM/Deep_Embedd_Clustering/assets/49087999/5cd4af4d-4cdb-4c2f-a048-9eb1d49ec0dc)

---

### Tips
*If you have any problem, you can send an email archercym@gmail.com or make an issue directly. We can discuss together.*
