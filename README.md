<div align="center">

# Sermo

QuotOS Aether 的独立 macOS 客户端

把 Aether 界面单独拿出来，配上自己的设置面板

**本仓库仅存放安装包，不包含源代码。**

</div>

---

## 这是什么

Aether 原本是 Lawlearn 里的一扇小窗，API 入口挂在主程序的设置页里。Sermo 把它单独拿出来做成一个独立应用：打开就是 Aether，不用先进主程序。

- **只有 Aether**：没有法条检索，没有主程序框架，窗口里就是那一个界面
- **设置就在顶上**：顶部栏「⚙ 设置」里填服务商与 API Key，存在本机，重启后还在
- **七家服务商**：DeepSeek、OpenAI、Moonshot、硅基流动、阿里通义、智谱、OpenRouter
- **界面随包携带**：断网也能打开，对话历史与图鉴存在本机

> [!IMPORTANT]
> 软件本身**不含任何 API 密钥**。首次打开请点右上角「⚙ 设置」，填入你自己的 API Key 与模型，保存后才能开始对话。

## 下载

| 平台 | 版本 | 系统要求 | 安装包 |
| --- | --- | --- | --- |
| macOS | **1.0.0** | macOS 14.0 及以上 | [Sermo-1.0.0.dmg](https://github.com/LynneScheutie/Sermo-download/releases/download/macOS-v1.0.0/Sermo-1.0.0.dmg) · 1.6 MB |

全部历史版本都在 [Releases](../../releases) 里。

## 安装

1. 下载 `.dmg` 后双击打开，把 `Sermo` 拖进「应用程序」文件夹。
2. 应用未经 Apple 公证，首次打开会提示「无法验证开发者」。到「系统设置 → 隐私与安全性」，在下方点「仍要打开」，再确认一次。
3. 如果提示「文件已损坏」，在终端执行下面这行再打开：

```bash
xattr -dr com.apple.quarantine /Applications/Sermo.app
```

4. 打开后点顶部「⚙ 设置」，填入 API Key 与模型，点「保存」。提示变成「已配置，当前生效：…」就说明可以用了。

## 校验值

| 文件 | SHA-256 |
| --- | --- |
| `Sermo-1.0.0.dmg` | `f268c5026edb8d06fc8bf87a84146eb1ae391d5fecd0dc46dbdb9f68ff7c00c1` |

macOS 上执行 `shasum -a 256 文件名` 对比即可。

## 关于源代码

源代码未公开，本仓库也不含任何源文件。

可以自由使用本软件，但不允许反编译、二次打包后以自己的名义分发，也不允许剥离版权声明。

## 问题反馈

在 [Issues](../../issues) 里提交，请说明系统版本、软件版本，以及具体在做什么操作时出的问题。
