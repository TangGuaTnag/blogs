# GitHub图床搭建

## 前言

- #### 此篇文章的作用：

  - 在github上创建一个图片仓库
  - 利用PicGo配置github图床环境
  - 利用PicGo上传图片
  - 在Typora上引用图片

- #### 工作环境：

  - 使用win10系统

  - 使用的软件如下：PicGo（上传图片，管理图片、生成链接）、Typora（使用图片链接）、github（用做图片仓库）

    

- #### GitHub图床优势：

  - 完全免费
  - 支持100MB以内大小图片（本人没有尝试过这么大的图片上传）
  - github开源平台，不用担心图片丢失

------

## 搭建图床

- #### 建立github仓库

  1. 首先先登录github，没有账号则创建一个。

  2. 创建仓库，Repositories旁边的New，开始创建一个新的仓库，如下：

     <img src="https://raw.githubusercontent.com/TangGuaTnag/image.io/main/github%E5%9B%BE%E7%89%87%E4%BB%93%E5%BA%93%E6%90%AD%E5%BB%BA-1.png" style="zoom:100%;" />

  3. 按照如下，name里面填写你的仓库名称，完成后点击Creat repository创建。

     <img src="https://raw.githubusercontent.com/TangGuaTnag/image.io/main/github%E5%9B%BE%E7%89%87%E4%BB%93%E5%BA%93%E6%90%AD%E5%BB%BA-2.png" style="zoom:100%;" />

- #### 生成token配置PicGo

  ​	因为PicGo需要将图像上传到Github仓库，所以需要用Github生成访问token使得PicGo可以正确的将图下上传至刚才创建的Github仓库。具体步骤如下：

  1. 点击个人头像，进入settings，如下

     ![](https://raw.githubusercontent.com/TangGuaTnag/image.io/main/github%E5%9B%BE%E7%89%87%E4%BB%93%E5%BA%93%E6%90%AD%E5%BB%BA-3.png)

  2. 进入 Developer settings，如下

     ![](https://raw.githubusercontent.com/TangGuaTnag/image.io/main/github%E5%9B%BE%E7%89%87%E4%BB%93%E5%BA%93%E6%90%AD%E5%BB%BA-4.png)

  3. 然后点击token管理，即Personal access tokens，在此界面可以删除token和新增token。

     ![](https://raw.githubusercontent.com/TangGuaTnag/image.io/main/github%E5%9B%BE%E7%89%87%E4%BB%93%E5%BA%93%E6%90%AD%E5%BB%BA-6.png)

  4. 然后在新的页面输入Note即备注，并选择repo权限，因为PicGo需要上传图片到仓库。

     ![](https://raw.githubusercontent.com/TangGuaTnag/image.io/main/github%E5%9B%BE%E7%89%87%E4%BB%93%E5%BA%93%E6%90%AD%E5%BB%BA-7.png)

  5. 然后点击生成token，Generate token

     ![](https://raw.githubusercontent.com/TangGuaTnag/image.io/main/github%E5%9B%BE%E7%89%87%E4%BB%93%E5%BA%93%E6%90%AD%E5%BB%BA-8.png)

  6. 生成token后，将token复制。**注意！**请勿泄露token，此token拥有repo权限，此页面token只显示一次，刷新或者再次进入token管理，无法查看之前创建的token，请及时复制。

     ![](https://raw.githubusercontent.com/TangGuaTnag/image.io/main/github%E5%9B%BE%E7%89%87%E4%BB%93%E5%BA%93%E6%90%AD%E5%BB%BA-9.png)

  7. 我们打开PicGo，点击图床设置，进入GitHub图床，设置仓库信息。仓库名称就是 你的名称/创建仓库的名称，token就是刚才复制的，分支即是仓库的分支，代表需要将图片上传到哪个分支，创建仓库成功后默认就是一个主干分支。

     ![](https://raw.githubusercontent.com/TangGuaTnag/image.io/main/github%E5%9B%BE%E7%89%87%E4%BB%93%E5%BA%93%E6%90%AD%E5%BB%BA-10.png)

     如果还不清楚可以进入github点击左上方的个人头像，即可查看已有的仓库，点击对应仓库可进入对应的仓库页面，如下图，xxxxxx/image.io即是仓库名称

     ![](https://raw.githubusercontent.com/TangGuaTnag/image.io/main/github%E5%9B%BE%E7%89%87%E4%BB%93%E5%BA%93%E6%90%AD%E5%BB%BA-11.png)

     分支名可以点击仓库名称，进入仓库查看，如下图的分支名则是main

     ![](https://raw.githubusercontent.com/TangGuaTnag/image.io/main/github%E5%9B%BE%E7%89%87%E4%BB%93%E5%BA%93%E6%90%AD%E5%BB%BA-12.png)

## 使用图床

- #### 	使用Typora

  1. 上述配置完成后即可在PicGo上传去上传图片啦，因为在Typora内使用图片，即上传Markdown即可。
  2. 自行google或者百度，下载Typora，就可以愉快的写博客啦！！

