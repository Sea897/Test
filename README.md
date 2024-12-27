# 人工智能复现
# 局部和非局部特征的深度融合，实现精确的滑坡制图

## 介绍
提出了一种融合局部和非局部特征以进行精确滑坡测绘的有效方法，该方法使用覆盖震后九寨沟的图像实现最先进的滑坡分割性能。

## 测试集结果

使用 1000 多张聚合九寨沟的无人机图像测试了我们的 DA-U-Net。

## 用法

  - 代码在 miniconda3：4.7.10-cuda10.1-cudnn7-ubuntu18.04 上测试，请从源码安装 tensorflow-gpu（1.9.0 版本）、Anaconda、CUDA9.0、CUDNN7.0。
  - 使用 pip 安装依赖项
   ```
   pip install -r requirements.txt
   ```
  - 或使用 anaconda 安装依赖项
  ```bash
  conda install -y --channel=https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/main --channel=https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/conda-forge \
        numpy==1.18.1 \
        opencv==3.4.2 \
        python==3.6.0 \
        tensorflow-gpu==1.9.0 \
    && conda clean -ya
  - If an error occurs, RUN apt-get update \
    && apt-get install -y --no-install-recommends \
        libglib2.0-dev=2.56.4-0ubuntu0.18.04.4 \
        python-qt4=4.12.1+dfsg-2 \
    && rm -rf /var/lib/apt/lists/*

  - run test code using `python -u 'test.py'`
  ```

## 数据集和模型

覆盖 6 个城镇的无人机图像是针对 2017 年 8 月 8 日中国九寨沟地震造成的山体滑坡获得的。


## 引用

```
@article{zhu2020deep,
  title={Deep Fusion of Local and Non-Local Features for Precision Landslide Recognition},
  author={Zhu, Qing and Chen, Lin and Hu, Han and Xu, Binzhi and Zhang, Yeting and Li, Haifeng},
  journal={arXiv preprint arXiv:2002.08547},
  year={2020}
}
```
