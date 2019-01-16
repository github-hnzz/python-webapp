>day01 环境搭建
>>确认Python的版本3.7.X
>>Python 异步架构 aiohttp
>>> $ pip install aiohttp
>>前端模板引擎 jinja2
>>> $ pip install jinja2
>>数据库安装 MYSQL 5.X (docker安装mysql最新版本)
>>>下载docker pull mysql
>>>启动docker run --name mysql -p 3306:3306 -e MYSQL_ROOT_PASSWORD=Lzslov123! -d mysql
>>>进入容器docker exec -it mysql bash
>>>登录msql mysql -u root -p
>>>添加远程登录账户
>>>>CREATE USER 'liaozesong'@'%' IDENTIFIED WITH mysql_native_password BY 'Lzslov123!';
>>>>GRANT ALL PRIVILEGES ON *.* TO 'liaozesong'@'%';
>>mysql的Python异步驱动程序aiomysql
>>> $ pip install aiomysql
>>在github上创建项目结构
>>>python-webapp/
>>>>backup/  --备份
>>>>conf/    --配置文件
>>>>dist/    --打包目录
>>>>www/     --web目录，存放.py文件
>>>>>static/        --存放静态文件
>>>>>templates/     --存放模板文件
>>>>ios/     --存放iOS APP工程
>>>>LICENSE/ --代码LICENSE 