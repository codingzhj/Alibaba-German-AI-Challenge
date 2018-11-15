# Alibaba-German-AI-Challenge
多通道城市图像分类
### 2018.11.15
* 第一次线上测评，利用两层卷积两层全连接网络制作的baseline线上accuracy达到0.702，当天排名第二名
  * 该baseline使用的时GD算法进行参数寻优，之后可以使用Adam算法进行替代观察线上成绩
* 根据官方给出的analysis文件中EDA的方法，plot出一个样本的18个通道的图像
* 由于dataset重视one-hot形式的label，所以利用一下代码计算出vali数据集中各类别的数量:
<pre><code>label_qty = np.sum(label, axis=0)</code></pre>
