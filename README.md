# 本项目实现了简单的人脸识别
## 项目介绍
本项目实现了电脑摄像头实时检测识别人脸，通过dlib实现人脸的检测，然后对检测出的人脸通过卷积神经网络实现识别，目前只能实现一个人脸的识别。
## 环境
```
python = 3.7.9
opencv-python = 4.4.0.46
dlib = 19.21.0
numpy = 1.19.2
tensorflow = 1.15.0
scikit-learn = 0.23.2
```
也可以通过以下命令直接配置环境
```
pip install -r requirements.txt
```
## 代码说明
1. getmyimg.py 是通过电脑摄像头采集自己的脸，数量可以在代码中修改，5000个就可以。
2. getOtherImg.py 是对下载的人脸数据集进行处理，生成我们需要的数据集格式
3. train.py 是对神经网络的训练代码
4. main.py 是检测代码
## 数据集
[LFW数据集](https://download.csdn.net/download/duzhongqiang/15176887)

## 训练步骤
1. 配置环境
2. 下载数据集
3. 运行getOtherImg.py对数据集进行处理
4. 运行getmyimg.py获取自己的人脸数据
5. 运行train.py训练
6. 运行main.py进行识别