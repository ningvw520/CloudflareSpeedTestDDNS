# CloudflareSpeedTestDDNS
使用CloudflareSpeedTest工具优选IP后自动DDNS到Cloudflare

## 更新日志
### v2.1 适配XIU2/CloudflareSpeedTest [v2.1.0](https://github.com/XIU2/CloudflareSpeedTest/releases/tag/v2.1.0) 修改ipv6测速策略

### v2.0 添加了多域名支持
可以在hostname中填入多个域名。使用[CloudflareSpeedTest](https://github.com/XIU2/CloudflareSpeedTest)工具得出优选IP列表后，脚本支持依次从速度最快的ip开始DDNS，域名数量可更具自己需求填写。
### 优化科学上网插件重启时机

## 原理
使用Cloudflare的API，将CloudflareSpeedTest工具优选到的最快IP，自动更新到指定域名上。

## [使用教程](https://blog.vbar.fun/archives/openwrt-ding-shi-you-xuan-cloudflareip-bing-geng-xin-dao-cloudflare)
详细使用教程请参考[详细教程](https://blog.vbar.fun/archives/openwrt-ding-shi-you-xuan-cloudflareip-bing-geng-xin-dao-cloudflare)

## 存在问题
.tk .ml .ga .cf .gq这几个域名可能存在无法调用CloudflareAPI。

## 感谢
感谢[XIU2](https://github.com/XIU2)给大家提供了[CloudflareSpeedTest](https://github.com/XIU2/CloudflareSpeedTest)这么方便的优选IP的工具。
https://github.com/XIU2/CloudflareSpeedTest
