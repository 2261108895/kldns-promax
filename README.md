## 由于原作者，觉得这个项目用途的确不大，已停更！
### 重构版由：XN工作室制作，项目地址：https://github.com/2261108895/kldns-promax/

# 快乐二级域名分发系统 （kldns v3.1.1）

## 此系统有哪些特点
* 1、增加AAAA解析ipv6网站
* 2、修复Cloudflare对接问题
* 3、美化UI
* 4、修复一些已知的问题
  ## 3.1.1 (2025.11.8)
* 目前支持的域名解析平台有
    *  dnspod
    *  cloudxns
    *  aliyun
    *  dnscom
    *  dnsla
    *  cloudxns
    *  DnsDun
* 多用户、多域名、多平台同时存在
* 界面简单、舒适，操作简单
## 3.1.1(2.0版本)
* 1、美化
* 2、加入多管理员功能
* 如果想要其他的美化请在/css/style.css中加入以下代码(要在安装完系统之后改代码，不然在安装的过程中会出现问题）
* 1️⃣ 全局过渡动画（Transition）
* 让按钮、输入框、卡片、hover 等交互带有轻微的淡入淡出与平滑过渡：
  * {
    transition: all 0.25s ease-in-out;
}

* 2️⃣ 圆角细化
* 让所有常见组件（按钮、输入框、模态框、卡片）都有一致的圆角风格
.btn, .card, .form-control, .modal-content, .navbar, .alert {
    border-radius: 16px !important;
}

* 3️⃣ 按钮点击动效（scale）
* 在点击按钮时轻微缩放（模仿 iOS 弹性动效）
.btn:active {
    transform: scale(0.96);
}

* 4️⃣ 模态框淡入动画
* 让登录框 / 弹出框淡入显示
.modal-content {
    animation: fadeInUp 0.4s ease both;
}
@keyframes fadeInUp {
    from {
        opacity: 0;
        transform: translateY(20px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

* 5️⃣ 毛玻璃容器入场动效
.frosted {
    animation: appear 0.6s ease-out;
}
@keyframes appear {
    from { opacity: 0; transform: scale(0.96); }
    to { opacity: 1; transform: scale(1); }
}

## 3.1.1 (1.0版本)
* 1、美化
* 2、修复Cloudflare对接问题
## 安装说明
* 1、程序的框架是Laravel 5.8，因此需要环境满足以下要求：
    * PHP >= 7.1.3
    * PHP OpenSSL 扩展
    * PHP PDO 扩展
    * PHP Mbstring 扩展
    * PHP Tokenizer 扩展
    * PHP XML 扩展
    * PHP Ctype 扩展
    * PHP JSON 扩展
    * PHP BCMath 扩展
* 2、环境必须支持伪静态

* Apache 伪静态配置
    * 确保 Apache 启用了 mod_rewrite 模块以支持 .htaccess 解析。
* Nginx 伪静态配置

        location / {
            try_files $uri $uri/ /index.php?$query_string;
        }

## 有问题反馈（XN工作室）
1、在使用中有任何问题，欢迎反馈给我，可以用以下联系方式跟我交流
* Github:https://github.com/2261108895/kldns-promax/
* 邮件(2261108895@qq.com)
* QQ: 2261108895
* QQ交流群：[1036288116](https://qm.qq.com/q/1BR89koO8w")
## 有问题反馈（原作者）
1、如果你需要程序支持其他域名解析平台，且该平台有api接口，可以联系我，我尽量添加！
2、在使用中有任何问题，欢迎反馈给我，可以用以下联系方式跟我交流
* Github:https://github.com/klsf/kldns
* 邮件(815856515@qq.com)
* QQ: 815856515
* QQ交流群：[383286818](http://shang.qq.com/wpa/qunwpa?idkey=5c50f31eb84481f05bbbeca6a0759a2e9763118f04dce5c6ca2e23652cb2a58b")
### 原版源码归原作者所有，重置版源码归XN工作室所有
