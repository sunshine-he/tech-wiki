# 容器技术和容器编排

## docker和docker-compose安装

### docker installation

!!! note "实验环境"
    本实验针对的是centos7及以上系统

- 环境准备
   
   **在终端执行如下命令：** :material-information-outline:{ title="请在root用户下执行" }

  ```console   
  yum -y install yum-utils device-mapper-persistent-data lvm2    
  ```
  
  <div class="termy">

  ```console
   # yum  install yum-utils device-mapper-persistent-data lvm2 -y
  ---> 100%
  Successfully installed.
  ```

  </div>


  
- 配置 yum 镜像仓库
   
   ```shell
   yum-config-manager --add-repo http://mirrors.163.com/.help/CentOS7-Base-163.repo
   yum-config-manager --add-repo http://mirrors.aliyun.com/docker-ce/linux/centos/docker-ce.repo
   ```

- 查询并安装指定版本
  
  ```shell

  1.  # yum list docker-ce --showduplicates|sort -r // 查询docker版本 
    
  2.  # yum install docker-ce-18.09.8 -y // 安装指定版本
      
  3.  # systemctl start docker && systemctl enable docker.service //启动docker
  ```


### docker-compose 安装

```shell
1.  # curl -L "https://github.com/docker/compose/releases/download/2.21.0/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
    
2.  # chmod a+x /usr/local/bin/docker-compose
    

3. Docker Compose 存放在 GitHub，不太稳定。

你可以也通过执行下面的命令，高速安装 Docker Compose。
curl -L https://get.daocloud.io/docker/compose/releases/download/v2.21.0/docker-compose-`uname -s`-`uname -m` > /usr/local/bin/docker-compose

4.github 韩国代理
curl -L "https://ghproxy.com/https://github.com/docker/compose/releases/download/2.21.0/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose

如下载不到，直接用下面地址
https://ghproxy.com/https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64
```

### 配置国内镜像源

**编辑/etc/docker/daemon.json 输入以下内容：**

```json
{
    "registry-mirrors": [
        "https://registry.hub.docker.com",
        "http://hub-mirror.c.163.com",
        "https://docker.mirrors.ustc.edu.cn",
        "https://registry.docker-cn.com"
    ]
}
```
 **==成功完成==**  :smile: