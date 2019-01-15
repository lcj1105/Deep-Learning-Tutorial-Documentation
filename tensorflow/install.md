## 环境配置
### 1. 安装Anaconda3  
由于anaconda里面自带很多包，而且可以构建多个环境，所以建议在Anaconda里面来管理pytorch、tensorflow等 

    下载地址：https://www.anaconda.com/download/#linux         

安装方法：sh  Anaconda2-4.2.0-Linux-x86_64.sh    一路点同意即可 

使用方法：https://www.jianshu.com/p/2f3be7781451 

使用技巧： 国内由于墙的原因，下载一些包特别慢，所以建议把conda源和pip源都切换成清华的 

    conda源切换： https://mirrors.tuna.tsinghua.edu.cn/help/anaconda/ 
    pip源切换： https://mirrors.tuna.tsinghua.edu.cn/help/pypi/    


### 2. 安装tensorflow 
由于之前某些代码是用的python2.7实现的，为了兼容代码，可以用conda创建一个python2.7的环境配置tensorflow 

执行以下脚本
```bash
conda create -n tensorflow pip python=2.7 # or python=3.3, etc. 
source activate tensorflow #激活tensorflow环境 
pip install tensorflow_gpu-1.4.0-cp27-none-linux_x86_64.whl  
```
 
要退出tensorflow环境也很简单，source deactivate 


### 4. 安装tensorboard 
Tensorboard是目前来说最好用的实时看训练过程的工具了，tensorflow下自带tensorboard，pytorch只需安装tensorboardX即可 

用法就是在集群输入： 

    tensorboard --logdir=【你的log文件夹，会自动搜索子文件夹】--port=9233【5000以后基本不会冲突】 

然后，打开浏览器，输入集群IP:9233，如10.5.34.21:9233 

详细用法： 

    pytorch使用tensorboardX：https://zhuanlan.zhihu.com/p/35675109 
    tensorflow使用tensorboard：https://zhuanlan.zhihu.com/p/26203726 
