# GIT使用步骤
1. 下载并安装 GIT 工具
2. 配置环境变量（如果在 CMD 中输入 git 能够执行，此步可以跳过）
`path=/git/cmd`
3. 生成密钥 `ssh-keygen -t rsa -C "登录邮箱"`
4. 全局配置 ```shell
git config --global user.email "登录邮箱"
git config --global user.name "用户名"
```

# github
1. 注册并验证邮箱
2. 配置密钥

# 码云
1. 注册
2. 配置密钥

# ideal+github
## 新项目上传到github中
1. 创建项目
2. `VCS -> import into Version Control -> Share project on GitHub -> 登录 -> 创建仓库 --> 选择上传的文件 --> 上传`
## 更新github中的项目
1. 提交变更的文件（临时存储变更状态）
`VCS -> commit -> 填写提交说明 -> 提交`
2. push到github仓库中
`VCS -> Git -> Push`
## 从github中克隆项目
1. `VCS -> Git -> Clone -> 填写仓库地址 -> 同意创建项目`

# 纯命令克隆
```shell
git init
git clone https://github.com/yaconit/JavaClassNotes.git
```