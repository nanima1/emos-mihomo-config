# Mihomo-emos 分流脚本

此脚本为 [Mihomo](https://github.com/MetaCubeX/mihomo) 生成完整的代理规则配置。

## 特性
- 自动按地区/倍率分类节点
- 集成丰富的 Rule Providers
- 支持 Emby、流媒体、AI 等多种服务分流
- 引用 [emos-proxy-rule](https://github.com/binaryu/emos-proxy-rule) 中的 emos 专用规则集

## 使用方法
将 `mihomoScript.js` 的内容作为 Mihomo 的配置生成脚本使用。

## 外部规则引用
本脚本通过 HTTP 直接加载以下远程规则，无需本地包含：
- [binaryu/emos-proxy-rule](https://github.com/binaryu/emos-proxy-rule) 的 `emos-mihomo.mrs`
- 其他众多 MetaCubeX 规则集
