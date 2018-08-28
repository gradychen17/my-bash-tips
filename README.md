# My bash tips
Bash tips

## 查看log文件找到指定文本并执行命令
`journalctl -n 1000 -u kubelet | grep -q 'PLEG is not healthy';echo $?|awk '/0/ { system("echo ok") }'`  *found and do something*
