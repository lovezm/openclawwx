# 🦞 iopenclawwx

![16181a6f94a93da778ca096235f2ff8b](https://github.com/user-attachments/assets/595044dc-2de7-4d87-8a8d-8b49c6515dba)

本项目主要是解决openclaw接入微信

通过 iopenclaw 的微信小程序，实现 **OpenClaw 与个人微信之间的通讯会话**。

在中国大陆环境下，Telegram、WhatsApp 等工具无法正常使用；飞书、钉钉配置复杂；企业微信仅支持企业账号；个人微信无法直接接入 OpenClaw 需要通过 Hook 或者 ipad/Mac协议接入 提升了封号风险并且接入繁琐。

**iopenclawwx 专为解决这一痛点而生。**

将 OpenClaw 与微信小程序连接，即可通过个人微信随时随地与 OpenClaw 对话。

---

## ✨ 核心优势

- ✅ 支持个人微信（无需企业认证）
- ✅ 极速接入（3 步完成配置）
- ✅ 完全免费（无需订阅，无需付费）
- ✅ 随时随地使用
- ✅ 安全认证（API Key 鉴权机制）
- ✅ 轻量插件架构（无侵入式扩展）

---

## 🚀 安装步骤

官网：https://iopenclaw.app

```bash
openclaw plugins install iopenclawwx
cd ~/.openclaw/extensions/iopenclawwx
npm run config-init  # 输入你的 API Key
openclaw gateway restart
```
```bash
[root@VM34698DE11A383E0 ~]# openclaw plugins install iopenclawwx

🦞 OpenClaw 2026.2.19-2 (45d9b20) — I speak fluent bash, mild sarcasm, and aggressive tab-completion energy.

│
◇  Doctor warnings ─────────────────────────────────────────────────────────────────────────╮
│                                                                                           │
│  - State dir migration skipped: target already exists (/root/.openclaw). Remove or merge  │
│    manually.                                                                              │
│                                                                                           │
├───────────────────────────────────────────────────────────────────────────────────────────╯
Downloading iopenclawwx…
Extracting /tmp/openclaw-npm-pack-9id2hN/iopenclawwx-0.0.2.tgz…
Installing to /root/.openclaw/extensions/iopenclawwx…
11:58:51 [plugins] plugins.allow is empty; discovered non-bundled plugins may auto-load: iopenclawwx (/root/.openclaw/extensions/iopenclawwx/index.ts). Set plugins.allow to explicit trusted ids.
Config overwrite: /root/.openclaw/openclaw.json (sha256 aa7b303ba098207dc576eec9a8d9781f9ef60780191a884ca9d1d1c48e870ae7 -> 0a1e2f43d5fb2722fe71e65db947655b54c229a892dcad83eaf0dd22432b8b2e, backup=/root/.openclaw/openclaw.json.bak, changedPaths=2)
Installed plugin: iopenclawwx
Restart the gateway to load plugins.
[root@VM34698DE11A383E0 ~]cd ~/.openclaw/extensions/iopenclawwx
[root@VM34698DE11A383E0 iopenclawwx]# npm run config-init

> iopenclawwx@0.0.2 config-init
> node scripts/config-init.js


════════════════════════════════════════
  iOpenClaw WX 配置初始化
════════════════════════════════════════
API Key（bot_xxx:secret）: b******************
✅ 已写入配置: /root/.openclaw/openclaw.json

ℹ 下一步执行: openclaw gateway restart
[root@VM34698DE11A383E0 iopenclawwx]# openclaw gateway restart
```
📱 使用方式
	1.	打开微信
	2.	扫描下方小程序码
	3.	登录并绑定
	4.	开始与 OpenClaw 对话

## 小程序码
![iOpenClaw 小程序码](https://github.com/lovezm/chatlog/blob/main/gh_498442564d0d_430.jpg?raw=true)

请我喝蜜雪
![3a8685b9f6660df9706496d99d01166c](https://github.com/user-attachments/assets/3f7a8993-ac55-40a7-a4d0-0340e59c868b)



