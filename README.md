# Ubuntu-18.04 -wget-403
使用wget命令从清华源下载anaconda的安装脚本，结果返回403错误，无法下载。
原因：服务器正在检查引用者，一些 HTTP 请求也会得到错误响应，因为它们会拒绝不以 Mozilla 开头或不包含 Wget 的用户代理
解决方法：输入命令
`wget --user-agent="Mozilla" https://mirrors.tuna.tsinghua.edu.cn/anaconda/archive/（某软件版本名）`
