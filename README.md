# firmoo 商城速度优化
## 根据 [PageSpeedLights](https://developers.google.com/speed/pagespeed/insights/?hl=zh-cn) 和 [WEGPAGETEST](https://webpagetest.org/easy.php)评测结果，主要分为3个方面问题：
### * TTFB超时
### * 图片过大
### * css文件过大

## 阶段一：缩短TTFB
TTFB:Time to First Byte 的缩写，指的是浏览器开始收到服务器响应数据的时间（后台处理时间+重定向时间），是反映服务端响应速度的重要指标。就像你问朋友了一个问题，你的朋友思考了一会儿才给你答案，你朋友思考的时间就相当于 TTFB。你朋友思考的时间越短，就说明你朋友越聪明或者对你的问题越熟悉。对服务器来说，TTFB 时间越短，就说明服务器响应越快

## 阶段二：建立图片处理服务器

## 阶段三：优化精简css文件
