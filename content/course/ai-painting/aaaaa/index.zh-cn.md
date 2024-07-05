---
title: "在HUGO文章底部添加微信和支付宝打赏功能"
date: 2024-07-02
weight: 192
draft: false
description: "了解如何在HUGO主题文件中添加打赏功能代码"
slug: "hugo-reward"
tags: ["HUGO","打赏","微信支付","支付宝"]
series: ["玩转HUGO"]
series_order: 1
---


> 网上有很多实现打赏功能的方法，本站使用的是添加HTML+CSS代码方式实现。

网上有很多实现打赏功能的方法，本站使用的是添加HTML+CSS代码方式实现，此方法简洁高效可适用于任何静态页面上。声明：下面的代码转自 “[方阁志](https://blog.imfang.net/web/119.html)”



## 添加HTML代码

找到并打开HUGO主题文件（一般在主题文件夹\layouts\partials\single\）添加一个reward.html，中添加如下代码，请把src=后面的打赏二维码图片改成你的图片地址，图片建议放在根目录下的static内。

```html
<div style="padding: 10px 0; margin: 20px auto; width: 100%; font-size:16px; text-align: center;">
        <button id="rewardButton" disable="enable" onclick="var qr = document.getElementById('QR'); if (qr.style.display === 'none') {qr.style.display='block';} else {qr.style.display='none'}">
            <span>打赏</span></button>
        <div id="QR" style="display: none;">
            <div id="wechat" style="display: inline-block">
                <a class="fancybox" rel="group">
                    <img id="wechat_qr" src="https://www.wusiqi.cn/WeChatPay.JPG" alt="WeChat Pay"></a>
                <p>微信打赏</p>
            </div>
            <div id="alipay" style="display: inline-block">
                <a class="fancybox" rel="group">
                    <img id="alipay_qr" src="https://www.wusiqi.cn/AliPay.JPG" alt="Alipay"></a>
                <p>支付宝打赏</p>
            </div>
        </div>
    </div>
```
## 添加CSS样式

找到并打开HUGO主题样式文件style.css/main.css（一般在主题文件夹\static\css），在最下方添加下面代码。

```css
#QR {
    padding-top:20px;
}
#QR a {
    border:0
}
#QR img {
    width:180px;
    max-width:100%;
    display:inline-block;
    margin:.8em 2em 0 2em
}
#rewardButton {
    border:1px solid #ccc;
    line-height:36px;
    text-align:center;
    height:36px;
    display:block;
    border-radius:4px;
    -webkit-transition-duration:.4s;
    transition-duration:.4s;
    background-color:#fff;
    color:#999;
    margin:0 auto;
    padding:0 25px
}
#rewardButton:hover {
    color:#f77b83;
    border-color:#f77b83;
    outline-style:none
}
```
打赏效果请参见本文章下方效果
