
 1. 首先是定位到目标文件夹，使用cd命令

$ cd  d:\github\我的网页 #git bash操作定位到文件夹，
#如果提示 bash： cd： no such file or directory,则按照下面的语句一步步定位
$ cd d: #定位d盘
$ cd data #定位d盘中的data文件夹
$ cd website #定位data中的website文件夹

2. 克隆github上的项目到本地

$ git clone https://github.com/zzzcola/test
# 操作完成后，website文件夹多了个名称为TEST的子文件夹，打开test，里面是github库上的内容被克隆到本地，存在一个 .git的文件夹。
# 将本地的网页所需的全部文件复制粘贴到TEST文件夹内，包括css、image、fonts、js等等，注意主网页必须命名为 index.html ，否则无法打开。

3. 上传网页到github库

$ cd TEST #注意，必须要定位到TEST文件夹，不然会报错
$ git add . #此处有空格和英文句号，目的是把TEST文件夹中自己复制粘贴的文件加进来 
$ git commit -m 'upload' #双引号里可以换成你需要的注释，这个操作上传数据
$ git push -u origin master #此操作目的是把本地仓库push到github上面，此步骤需要你输入github帐号和密码
