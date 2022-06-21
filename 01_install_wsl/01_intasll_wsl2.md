# 安装WSL

参考：[旧版 WSL 的手动安装步骤](https://docs.microsoft.com/zh-cn/windows/wsl/install-manual)

## WSL手动安装

1. 启用适用于 Linux 的 Windows 子系统

    ``` powershell
    dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
    ```

2. 启用虚拟机功能\

    ``` powershell
    dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
    ```

3. 下载 WSL 更新包

   [适用于 x64 计算机的 WSL2 Linux 内核更新包](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi)

4. 将 WSL 2 设置为默认版本

    ``` powershell
    wsl --set-default-version 2
    ```

5. 查看发行版本

   ``` shell
   wsl --list --online
   ```

6. 安装发行版本

   ``` shell
   wsl --install -d <DistroName>
   ```

7. 或者将 发行版 下载到指定文件夹，然后安装，例如

    [utunbtu 20.04](https://aka.ms/wslubuntu2004)

8. 将下载文件夹后缀名改为 zip，然后解压到指定文件夹，就可以实现 发行版不安装在系统盘
