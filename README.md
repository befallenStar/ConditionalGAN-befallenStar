# Jittor 草图生成风景比赛 baseline
![主要结果](https://s3.bmp.ovh/imgs/2022/04/19/440f015864695c92.png)
## 简介
本项目包含了第四届计图人工智能挑战赛 - 热身赛的代码实现。本项目的特点是：采用了 XX 方法对 YY 处理，取得了 ZZ 的效果。

## 安装
本项目可在 1 张 3060 上运行，训练时间约为 X 小时。

#### 运行环境
- Windows 11
- python >= 3.8
- jittor >= 1.3.8

#### 安装依赖
执行以下命令安装 python 依赖
```
pip install -r requirements.txt
```

#### 预训练模型
预训练模型模型下载地址为 https:abc.def.gh，下载后放入目录 `<root>/weights/` 下。

## 数据预处理
将数据下载解压到 `<root>/data` 下，执行以下命令对数据预处理：
```
bash scripts/prepross.sh
```

## 训练
单卡训练可运行以下命令：
```
bash scripts/train.sh
```

## 推理
生成测试集上的结果可以运行以下命令：

```
bash scripts/test.sh
```

## 致谢
此项目基于论文 *A Style-Based Generator Architecture for Generative Adversarial Networks* 实现，部分代码参考了 [jittor-gan](https://github.com/Jittor/gan-jittor)。
