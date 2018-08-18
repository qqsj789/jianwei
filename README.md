## ShawnMark/jianwei 项目能给你什么？
- 程序化模拟自动登陆见微数据网站
- 自动获取所有符合要求的文件信息
- 自动导出到MongoDB数据库或是CSV文件

## 该项目的配置要求？
- Python V3.6+（必须）
- Scrapy（必须）
- PyMongo（如无，可选择其他存储形式）

## 该项目的启动设置？
1. 修改./jianwei/settings.py文件
    - 见微数据的用户名、密码（必须）
    - MongoDB的存储、CSV导出的修改（如有必要）
    - 其他，比如下载延时（防止被封）等
2. 修改./jianwei/spiders/spider_xml.py文件
    - 修改是否自动生成字段.txt文件
    - 修改是否自动打印窗口实时输出
    - 修改 if... yield...语句（默认下载100多页的2000多只股票的IPO信息)
3. 其他

## TO-DO
- 更完善的搜索API配置
- PDF内容页的信息提取
- 其他  