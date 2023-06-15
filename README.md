## 项目介绍

> `EasyAdmin8` 基于 [`EasyAdmin`](https://gitee.com/zhongshaofa/easyadmin) 的基础上更新 ThinkPHP 框架到 8.0 ，PHP 最低版本要求不低于 8.0
>
> ThinkPHP v8.0 和 layui v2.8.x 的快速开发的后台管理系统。
>
> 演示地址：[easyadmin8.wolfcode.top](http://easyadmin8.wolfcode.top)

## 安装教程

> EasyAdmin8 使用 Composer 来管理项目依赖。因此，在使用 EasyAdmin8 之前，请确保你的机器已经安装了 Composer。

#### 通过 Composer 创建项目`建议`

`composer install`

#### 通过git下载安装包，composer安装依赖包

```
1.下载安装包

  git clone https://github.com/wolf-leo/easyAdmin8

  或者

  git clone https://gitee.com/wolf18/easyAdmin8

2.安装依赖包（确保 PHP 版本 >= 8.0）

  composer install
  
3. 拷贝 .example.env 文件重命名名为 .env

4.配置伪静态(以 Nginx 为例)
  
  location / {
    if ( !-e $request_filename){
        rewrite ^/(.*)$ /index.php?s=$1 last;
        break;
    }
  }

```

## 界面预览

### 
<center>
  <img src="public/static/common/images/easyadmin8-01.png" />
</center>

### 
<center>
  <img src="public/static/common/images/easyadmin8-02.png" />
</center>

### 
<center>
  <img src="public/static/common/images/easyadmin8-03.png" />
</center>

## 项目特性

* 快速CURD命令行
    * 一键生成控制器、模型、视图、JS文件
    * 支持关联查询、字段设置等等
* 基于`auth`的权限管理系统
    * 通过`注解方式`来实现`auth`权限节点管理
    * 具备一键更新`auth`权限节点，无需手动输入管理
    * 完善的后端权限验证以及前面页面按钮显示、隐藏控制
* 完善的菜单管理
    * 分模块管理
    * 无限极菜单
    * 菜单编辑会提示`权限节点`
* 完善的上传组件功能
    * 本地存储
    * 阿里云OSS`建议使用`
    * 腾讯云COS
    * 七牛云OSS
* 完善的前端组件功能
    * 对layui的form表单重新封装，无需手动拼接数据请求
    * 简单好用的`图片、文件`上传组件
    * 简单好用的富文本编辑器`ckeditor`
    * 对弹出层进行再次封装，以极简的方式使用
    * 对table表格再次封装，在使用上更加舒服
    * 根据table的`cols`参数再次进行封装，提供接口实现`image`、`switch`、`list`等功能，再次基础上可以自己再次扩展
    * 根据table参数一键生成`搜索表单`，无需自己编写
* 完善的后台操作日志
    * 记录用户的详细操作信息
    * 按月份进行`分表记录`
* 一键部署静态资源到OSS上
    * 所有在`public\static`目录下的文件都可以一键部署
    * 一个配置项切换静态资源（oss/本地）
* 上传文件记录管理
* 后台路径自定义，防止别人找到对应的后台地址

## 免责声明

> 所有协议遵循 [`EasyAdmin`](https://gitee.com/zhongshaofa/easyadmin)
>
> 任何用户在使用 `EasyAdmin8` 后台框架前，请您仔细阅读并透彻理解本声明。您可以选择不使用`EasyAdmin8`后台框架，若您一旦使用`EasyAdmin8`后台框架，您的使用行为即被视为对本声明全部内容的认可和接受。

* `EasyAdmin8`后台框架是一款开源免费的后台快速开发框架 ，主要用于更便捷地开发后台管理；其尊重并保护所有用户的个人隐私权，不窃取任何用户计算机中的信息。更不具备用户数据存储等网络传输功能。
* 您承诺秉着合法、合理的原则使用`EasyAdmin8`后台框架，不利用`EasyAdmin8`后台框架进行任何违法、侵害他人合法利益等恶意的行为，亦不将`EasyAdmin8`后台框架运用于任何违反我国法律法规的 Web 平台。
* 任何单位或个人因下载使用`EasyAdmin8`后台框架而产生的任何意外、疏忽、合约毁坏、诽谤、版权或知识产权侵犯及其造成的损失 (包括但不限于直接、间接、附带或衍生的损失等)，本开源项目不承担任何法律责任。
* 用户明确并同意本声明条款列举的全部内容，对使用`EasyAdmin8`后台框架可能存在的风险和相关后果将完全由用户自行承担，本开源项目不承担任何法律责任。
* 任何单位或个人在阅读本免责声明后，应在《MIT 开源许可证》所允许的范围内进行合法的发布、传播和使用`EasyAdmin8`后台框架等行为，若违反本免责声明条款或违反法律法规所造成的法律责任(包括但不限于民事赔偿和刑事责任），由违约者自行承担。
* 如果本声明的任何部分被认为无效或不可执行，其余部分仍具有完全效力。不可执行的部分声明，并不构成我们放弃执行该声明的权利。
* 本开源项目有权随时对本声明条款及附件内容进行单方面的变更，并以消息推送、网页公告等方式予以公布，公布后立即自动生效，无需另行单独通知；若您在本声明内容公告变更后继续使用的，表示您已充分阅读、理解并接受修改后的声明内容。

