# FkShittyAirportRules
# MYrules.yaml 配置文件说明

## 简介
本 `MYrules.yaml` 是专门为小白用户（我）准备的配置模板，用于优化网络代理配置。  
它可以替换机场陈旧简陋的分流规则，借助每日更新的开源规则集，为用户提供更高效、精准的代理服务。

## 使用说明

### 替换订阅地址
在 `proxy-providers` 部分，找到 `Airport0` 的配置项，将其中 `url` 字段的 `"机场订阅地址"` 替换为你自己的机场订阅链接。示例如下：
```yaml
proxy-providers:
  Airport0:
    type: http
    path: ./ProxySet/MYrules/MYrules.yaml
    url: "你的机场订阅链接" #替换为实际的订阅链接
    health-check:
      enable: true
      url: http://www.gstatic.com/generate_204
      interval: 300
```
## 说明
### 规则集使用说明
本项目规则集（RULE-SET）的数据主要来源于项目 [@Loyalsoldier/v2ray-rules-dat](https://github.com/Loyalsoldier/v2ray-rules-dat)。
本项目使用了 [Loyalsoldier/clash-rules](https://github.com/Loyalsoldier/clash-rules) 开源规则集，该规则集为 Clash 配置提供了丰富且实用的规则列表，涵盖了直连域名、代理域名、广告域名等多种类型的规则，能有效帮助用户对网络流量进行分流和管控。

### 测试情况说明
目前本项目的规则配置仅在以下两款软件中进行了测试：
- **Clash Verge**
- **Clash Meta**

### 此Readme由豆包女士与我共同创作
*关注豆包喵~*  
*关注豆包谢谢喵～(=^‥^) ノ*
