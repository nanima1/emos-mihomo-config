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

1. 启动 [**Clash Party**](https://github.com/mihomo-party-org/clash-party) 客户端
2. 进入**覆写**页面
3. 点击 **新建** 或 **导入** 按钮
4. 选择 **链接导入** 或 **从 URL 导入**
5. 输入本仓库的覆写脚本链接：https://raw.githubusercontent.com/nanima1/emos-mihomo-config/main/mihomoScript-emos.js
6. 确认保存后，前往**订阅管理**，将本次导入的覆写脚本**绑定**到你正在使用的 Mihomo 订阅上

> ⚠️ 绑定后请**手动更新一次订阅**，使覆写规则生效。

### 📱 安卓端（FlClash）

1. 打开 [**FlClash**](https://github.com/chen08209/FlClash) 客户端
2. 点击底部导航栏 **配置**
3. 点击页面顶部的 **覆写** 标签页
4. 点击右下角 **添加** → 选择 **通过 URL 导入**
5. 在弹出的输入框中粘贴：https://raw.githubusercontent.com/nanima1/emos-mihomo-config/main/mihomoScript-emos.js
6. 点击 **确定** 或 **提交** 完成导入
7. 返回覆写列表，**勾选启用**刚导入的 `mihomoScript-emos.js`

> 📌 启用后，Emby 相关流量将自动按规则分流，无需手动修改节点。

---

## 🔗 外部规则引用

本脚本引用了以下外部开源规则仓库：

| 规则名称 | 引用地址 | 说明 |
|:---|:---|:---|
| `emos-mihomo.mrs` | [binaryu/emos-proxy-rule](https://github.com/binaryu/emos-proxy-rule) | Emby 专用域名规则集 |
| `Emby.mrs` / `Emby_ip.mrs` | [666OS/rules](https://github.com/666OS/rules)（原始 Emby 规则） | 备用兼容 |

上述规则均**直接通过 URL 远程加载**，本仓库仅提供覆写脚本的整合入口。

---

## 📁 项目结构
emos-mihomo-config/

├── mihomoScript-emos.js ← 主覆写脚本（含 emos 专用规则）

└── README.md ← 本说明文档

如需自行修改规则，请 fork 本仓库后编辑 `mihomoScript-emos.js` 中的 `ruleProviders` 对象。

---

## ⚠️ 免责声明

- 本项目**仅提供规则覆写脚本**，不含任何代理节点或订阅服务
- 所有外部规则文件的版权归**原作者**所有（详见上方表格）
- 因客户端配置错误、网络环境差异导致的分流失效问题，本仓库**不承担责任**
- 使用前请确保已拥有**合法的代理订阅**，并遵守当地法律法规

---

## ⚖️ 许可证

本项目脚本采用 [MIT License](LICENSE) 开源，引用到的外部开源规则集**均保留原仓库的许可证**，请勿用于任何违法用途。

---

**🎯 一键配好 Emby 分流，观影更丝滑！**
