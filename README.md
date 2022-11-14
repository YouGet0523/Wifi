# Wifi
获取连接过的所有wifi账号密码

限制：仅用于笔记本（拥有wifi功能的电脑。），获取链接过的所有wifi账号和密码


cmd获取所有wifi命令
for /f "skip=9 tokens=1,2 delims=:" %i in ('netsh wlan show profiles') do  @echo %j | findstr -i -v echo | netsh wlan show profiles %j key=clear


脚本直接在Windows运行即可。
