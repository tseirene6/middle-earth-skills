# 可选阅读工具

这些工具辅助管理与阅读，不是四个 Skill 必须全部安装的依赖。
## 两条路线

| 路线 | 文献管理 | 阅读与翻译 | 自己的思考 |
|---|---|---|---|
| 浏览器阅读 | Zotero 收集、分类和引用 | 直接打开论文网页或 PDF，按需查词或双语对照 | Obsidian 或其他 Markdown 编辑器 |
| Zotero 阅读 | Zotero 收集和分类 | 内置 PDF 阅读器，按需安装兼容翻译插件 | Obsidian 或其他 Markdown 编辑器 |

论文能在浏览器打开时，可以直接阅读和翻译，也可以不先下载至 Zotero。Zotero 也可以主要承担文献库管理。参见 [Zotero 官方入门](https://www.zotero.org/support/quick_start_guide)。

## 浏览器辅助

[沙拉查词](https://github.com/crimx/ext-saladict) 适合词义与选中文本查询；[沉浸式翻译](https://immersivetranslate.com/zh-Hans/docs/) 提供网页双语阅读与 PDF 翻译等功能。具体 PDF 阅读器、浏览器权限和扩展版本影响表现。翻译辅助理解，关键条件、否定、量词与公式仍需核对原文。沉浸式翻译不用开会员（如果你不追求特别精准的翻译的话~）

## Zotero 与 PDF2zh

按自己的版本选择兼容插件，不要求一定在 Zotero 内翻译。作者私人环境中的“PDF2zh 一键连接”是本地服务启动快捷方式：检查服务健康状态，按需启动 Python 服务，并打开本地页面。它不是独立翻译引擎，也不是 Skill 安装器。


## 书生 API

书生是可尝试的模型服务选项（也是我本人尝试过的一个模型，书生是暂时免费的，但是速度比不上deepseek api），不是必要依赖。
官方 [Chat Completions 文档](https://internlm.intern-ai.org.cn/doc/docs/Chat/) 提供接口示例，并说明只兼容 OpenAI Python SDK 的部分方法；[Messages API](https://internlm.intern-ai.org.cn/doc/docs/API_DOCUMENTATION_ZH/) 使用另一种请求格式。客户端支持某一种协议，不代表支持所有参数或另一协议。

注意！！！官方 [迁移公告](https://internlm.intern-ai.org.cn/doc/docs/服务迁移说明/)（2026-10-26）指出：2026-11-09 起原入口仅保留 Intern-S2，其他模型 ID 转发到该模型；2027-01-26 起原入口停用，转至书生·端砚。新配置应首先查看 [书生·端砚](https://discovery.intern-ai.org.cn/) 科研模型入口及当前文档。

接入前检查客户端可否配置端点、模型名、鉴权和请求参数，然后用短文本验证响应解析与错误处理。API 已有文档、账户能够调用、某插件接入成功是三种不同状态。密钥只在本地配置，不写入仓库、截图或日志；价格与额度以使用时的平台信息为准。
