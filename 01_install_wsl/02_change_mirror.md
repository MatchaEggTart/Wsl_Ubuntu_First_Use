# Ubuntu替换清华镜像源

1. 首先安装两个包

    ``` shell
    sudo apt install apt-transport-https -y
    ```

    ``` shell
    sudo apt install ca-certificates -y
    ```

2. [Ubuntu 镜像使用帮助](https://mirror.tuna.tsinghua.edu.cn/help/ubuntu/)

3. 更新镜像

    ``` shell
    sudo apt-get update -y
    ```
