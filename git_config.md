# git 安装配置 ssh

## 1.生成密钥对 qq


### 1.1切换当前路径为家目录

```bash
cd ~
```
### 1.2 查看当前是否有git的ssh密钥存在
```bash
find ./ -name .ssh
```
> 如果未查询到.ssh文件夹，则未配置，直接到下一步配置即可；若存在.ssh文件夹，查看里面是否存在相关密钥文件
```bash
ls
```
> example
```
id_rsa  id_rsa.pub
```
> 若存在相关密钥配置文件，则说明已配置过，则无需在配置，若不存在，则进行下一步

### 1.3生成.ssh密钥对
```
ssh-keygen -t rsa -C "404327065@qq.com"
```
>