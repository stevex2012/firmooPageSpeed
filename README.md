# firmoo 商城速度优化
## 根据 [PageSpeedLights](https://developers.google.com/speed/pagespeed/insights/?hl=zh-cn) 和 [WEGPAGETEST](https://webpagetest.org/easy.php)评测结果，主要分为3个方面问题：
* ### 1.TTFB超时
* ### 2.图片过大
* ### 3.css文件过大

## 阶段一：缩短TTFB
TTFB:Time to First Byte 的缩写，指的是浏览器开始收到服务器响应数据的时间（后台处理时间+重定向时间），是反映服务端响应速度的重要指标。就像你问朋友了一个问题，你的朋友思考了一会儿才给你答案，你朋友思考的时间就相当于 TTFB。你朋友思考的时间越短，就说明你朋友越聪明或者对你的问题越熟悉。对服务器来说，TTFB 时间越短，就说明服务器响应越快
### TTFB 过长的原因：
* 用户距离服务器地理位置过长，或者用户和服务器之间的网络不好
* 浏览器中保留了过多的cookie，每次请求都会带上cookie，服务器处理cookie也会增加时间
* 服务端渲染请求后端api接口超时，数量过多都会增加耗时

1.排查服务端请求接口，移除和seo不相关的接口在客户端请求，测试服务端渲染接口请求速度响应，列出时间过长的接口，让后端优化

2.排查浏览器cookie，删除不必要多余cookie


## 阶段二：建立图片处理服务器



## 阶段三：优化精简css文件
