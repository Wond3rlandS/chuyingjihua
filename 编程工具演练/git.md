# Git基础配置

```shell
cp contrib/completion/git-completion.bash /etc/bash_completion.d/

. /etc/bash_completion

~/.bash/profile /etc/bashrc

if [ -f /etc/bash_completion ]; then
. /etc/bash_completion
fi

git config --system/global/local

# user
git config --global user.name "Zhang San"
git config --global user.email "zhangsan123@huawei.com"

# CRLF and LF
git config --global core.autocrlf true // on Windows
git config --global core.autocrlf input // on Linux
git config --global core.autocrlf false // on Windows only

# 中文编码支持
git config --global gui.encoding utf-8
git config --global i18n.commitencoding utf-8
git config --global i18n.logoutputencoding utf-8

# 显示路径中的中文：
git config --global core.quotepath false

# http/https协议认证
# 设置口令缓存：
git config --global credential.helper store
# 添加HTTPS证书信任：
git config http.sslverify false

# ssh认证
ssh-keygen -t rsa -C zhangsan123@huawei.com

# git 命令
git clone/diff/status/add/rm/mv/commit/push/log
git branch
git branch/checkout -b
git branch -d
git checkout
git pull/merge/reset/checkout/rebase



```
