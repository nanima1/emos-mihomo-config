# 🚀 emos-mihomo-config

适用于 `Mihomo` 内核的 **Emby 专项分流覆写脚本**。

> 📌 内置专用 Emby 域名规则集 `emos-mihomo.mrs`，可一键将 Emby 相关流量精准分流至指定节点，避免重复配置，提升观影体验。

---

## ✨ 功能特性

- ✅ **Emby 专用分流**：集成 [`emos-proxy-rule`](https://github.com/binaryu/emos-proxy-rule) 规则集，自动识别 Emby 域名流量
- ✅ **双平台覆写**：支持 PC 端 `Clash Party` 与 Android 端 `FlClash` 一键导入
- ✅ **动态更新**：规则通过 URL 远程加载，随上游仓库持续更新

---

## 📥 使用方法（覆写脚本）

### 💻 PC 端（Clash Party）

1. 启动 [**Clash Party**](https://github.com/mihomo-party-org/clash-party) 客户端[reference:0]
2. 进入**覆写**页面
3. 点击 **新建** 或 **导入** 按钮[reference:1]
4. 选择 **链接导入** 或 **从 URL 导入**
5. 输入本仓库的覆写脚本链接：
