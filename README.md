# seleniumtaobao
1.使用scrapy+selenium+phantomjs爬取淘宝商品并存储到Mongodb中
2.selenium+phantomjs配合模拟浏览器加载动态网页,最终返回结果给spider处理
3.爬取的商品关键字、爬取页数可通过settings.py配置文件配置,支持多关键字


备注:
关于环境配置安装：
1.安装scrapy，直接用sudo pip install scrapy
2.安装selenium 通过pip直接安装:sudo pip install selenium
3.phantomjs安装 可以直接使用apt安装 sudo apt-get install phantomjs，但可能会安装不全导致使用报错。
在ubuntu16.04中报错Unable to load Atom 'find_elements'，可通过官网下载对应的二进制文件，解压后
cp到/usb/bin下或者在/usb/bin下建立个名字叫phantomjs的软链接指向实际的可执行文件也可
4.mongodb安装 ubuntu下 sudo apt-get install mongodb
5.pymongo安装 通过pip安装 sudo pip3 install pymongo


环境安装完毕后在工程目录下运行：scrapy crawl taobao即可开始爬取

