### VSCode+PicGo+阿里云图床
==这是一段高亮的文本。==

#### 1.  阿里云OSS服务配置

1.  创建存储建Bucket
2.  将右边的访问域名中的“外网访问”的“Bucket域名”记下来，如：cunchutong.oss-cn-beijing.aliyuncs.com。
3.  点击头像，选择AccessKey管理，创建一个AccessKey，并且将AccessKey和AccessKey Secret记下来

### 2.配置PicGo

1.  搜索安装插件，然后点击Extension Settings进入PicGo的配置
2.  设置：Picgo › Pic Bed: Current，将图床类型设置为：aliyun
3.  第一步：Access Key ID\
    第二步：Access Key Secret\
    第三步:  Area 存储桶所在区域，填写英文或pinyin，如：oss-cn-beijing\
    第四步:  Bucket存储桶名称，如：xincunqianjie\
    第五步:  外网访问地址，如:<https://cunchutong.oss-cn-beijing.aliyuncs.com>\
    第六步:  图片文件夹，可不写，如：img/

### 3.PicGo 使用方法和快捷键

1.  在Windows中启动截图 Windows + Shift + S
2.  从剪贴板上传图像 Ctrl + Alt + U
3.  U从资源管理器上传图像 Ctrl + Alt + E&#x20;
4.  从输入框上传图像 Ctrl + Alt + O

***

### VSCode+PicGo+Github配置图床

#### 1. Github存储桶服务配置

1.  新增存储桶，注意权限选择公共 Public
2.  点击右上角账号头像，选择设置 Settings
3.  在设置页面左边菜单找到：Developer Settings
4.  在左边菜单找到Personal access tokens下的 tokens(classic)
5.  点击New personal access token (classic) 添加新的token
6.  设置token\
    1.Note 设置token名称，必填\
    2.Expiration 设置tiken过期时间\
    3.选项框中的repo下的所有项目必选\
    4.提交 Generate token
7.  复制生成的token

### 2.配置PicGo

1.  设置：Picgo › Pic Bed: Current，将图床类型设置为：github
2.  Branch 分支名称   master
3.  Custom Url 自定义网址 可为空
4.  &#x20;Path 路径 可为空 也可指定如\:img/
5.  &#x20;Repo 回购 如\:xincunhoujie/tupian
6.  &#x20;Token 密匙 \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*

#### 3.解决上传到GitHub的图片无法显示的方法‌：

1.  **修改hosts文件‌**：
2.  &#x20;打开hosts文件（通常位于C:\Windows\System32\drivers\etc），使用管理员权限打开。
3.  **添加以下内容**：
4.  185.199.108.133 githubusercontent.com\
    185.199.108.133 raw\.githubusercontent.com
5.  刷新IP映射 运行->cmd>ipconfig/flushdns  (此步可选)\
    其他命令：ipconfig /displaydns # 显示dns缓存\
    &#x20;               ipconfig /renew # 重请从DHCP服务器获得IP


