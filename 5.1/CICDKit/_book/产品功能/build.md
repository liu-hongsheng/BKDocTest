### 构件管理 {#build}

流水线中执行归档或镜像推送操作的程序包，会统一存放一份在构件仓库中。构件仓库分为通用仓库和镜像仓库两种，所有类型的二进制程序包存放在通用仓库，Docker 镜像存放在镜像仓库。通用仓库可复制链接进行程序包下载，镜像仓库则可通过 Docker Image 的进行 pull 获取镜像。
![](/assets/bk-cicdkit-21.png)

![](/assets/bk-cicdkit-22.png)
