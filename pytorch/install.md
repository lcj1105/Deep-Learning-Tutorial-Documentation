## 环境配置
### 1. 安装Anaconda3  
由于anaconda里面自带很多包，而且可以构建多个环境，所以建议在Anaconda里面来管理pytorch、tensorflow等 

    下载地址：https://www.anaconda.com/download/#linux         

安装方法：sh  Anaconda2-4.2.0-Linux-x86_64.sh    一路点同意即可 

使用方法：https://www.jianshu.com/p/2f3be7781451 

使用技巧： 国内由于墙的原因，下载一些包特别慢，所以建议把conda源和pip源都切换成清华的 

    conda源切换： https://mirrors.tuna.tsinghua.edu.cn/help/anaconda/ 
    pip源切换： https://mirrors.tuna.tsinghua.edu.cn/help/pypi/    


### 2. 安装pyTorch 
由于之前已经装好了anaconda，所以装pytorch就很简单了，一句话搞定： 

    conda install pytorch torchvision -c pytorch 

PS:  有时候网速不给力，可以尝试离线安装 

离线安装方法： conda install pytorch-0.4.0-py36_cuda8.0.61_cudnn7.1.2_1.tar.bz2 
