<div align="center">

![new-api](/web/public/logo.png)

# New API

🍥 **新一代大模型网关与AI资产管理系统**

<p align="center">
  <strong>中文</strong> | 
  <a href="./README.en.md">English</a> | 
  <a href="./README.fr.md">Français</a> | 
  <a href="./README.ja.md">日本語</a>
</p>

<p align="center">
  <a href="https://raw.githubusercontent.com/Calcium-Ion/new-api/main/LICENSE">
    <img src="https://img.shields.io/github/license/Calcium-Ion/new-api?color=brightgreen" alt="license">
  </a>
  <a href="https://github.com/Calcium-Ion/new-api/releases/latest">
    <img src="https://img.shields.io/github/v/release/Calcium-Ion/new-api?color=brightgreen&include_prereleases" alt="release">
  </a>
  <a href="https://github.com/users/Calcium-Ion/packages/container/package/new-api">
    <img src="https://img.shields.io/badge/docker-ghcr.io-blue" alt="docker">
  </a>
  <a href="https://hub.docker.com/r/CalciumIon/new-api">
    <img src="https://img.shields.io/badge/docker-dockerHub-blue" alt="docker">
  </a>
  <a href="https://goreportcard.com/report/github.com/Calcium-Ion/new-api">
    <img src="https://goreportcard.com/badge/github.com/Calcium-Ion/new-api" alt="GoReportCard">
  </a>
</p>

<p align="center">
  <a href="https://trendshift.io/repositories/8227" target="_blank">
    <img src="https://trendshift.io/api/badge/repositories/8227" alt="Calcium-Ion%2Fnew-api | Trendshift" style="width: 250px; height: 55px;" width="250" height="55"/>
  </a>
</p>

<p align="center">
  <a href="#-快速开始">快速开始</a> •
  <a href="#-主要特性">主要特性</a> •
  <a href="#-部署">部署</a> •
  <a href="#-文档">文档</a> •
  <a href="#-帮助支持">帮助</a>
</p>

</div>

## 📝 项目说明

> [!NOTE]  
> 本项目为开源项目，在 [One API](https://github.com/songquanpeng/one-api) 的基础上进行二次开发

> [!IMPORTANT]  
> - 本项目仅供个人学习使用，不保证稳定性，且不提供任何技术支持
> - 使用者必须在遵循 OpenAI 的 [使用条款](https://openai.com/policies/terms-of-use) 以及**法律法规**的情况下使用，不得用于非法用途
> - 根据 [《生成式人工智能服务管理暂行办法》](http://www.cac.gov.cn/2023-07/13/c_1690898327029107.htm) 的要求，请勿对中国地区公众提供一切未经备案的生成式人工智能服务

---

## 🤝 我们信任的合作伙伴

<p align="center">
  <em>排名不分先后</em>
</p>

<p align="center">
  <a href="https://www.cherry-ai.com/" target="_blank">
    <img src="./docs/images/cherry-studio.png" alt="Cherry Studio" height="80" />
  </a>
  <a href="https://bda.pku.edu.cn/" target="_blank">
    <img src="./docs/images/pku.png" alt="北京大学" height="80" />
  </a>
  <a href="https://www.compshare.cn/?ytag=GPU_yy_gh_newapi" target="_blank">
    <img src="./docs/images/ucloud.png" alt="UCloud 优刻得" height="80" />
  </a>
  <a href="https://www.aliyun.com/" target="_blank">
    <img src="./docs/images/aliyun.png" alt="阿里云" height="80" />
  </a>
  <a href="https://io.net/" target="_blank">
    <img src="./docs/images/io-net.png" alt="IO.NET" height="80" />
  </a>
</p>

---

## 🙏 特别鸣谢

<p align="center">
  <a href="https://www.jetbrains.com/?from=new-api" target="_blank">
    <img src="https://resources.jetbrains.com/storage/products/company/brand/logos/jb_beam.png" alt="JetBrains Logo" width="120" />
  </a>
</p>

<p align="center">
  <strong>感谢 <a href="https://www.jetbrains.com/?from=new-api">JetBrains</a> 为本项目提供免费的开源开发许可证</strong>
</p>

---

## 🚀 快速开始

### 使用 Docker Compose（推荐）

1. 第三方模型 **gpts** （gpt-4-gizmo-*）
2. 第三方渠道[Midjourney-Proxy(Plus)](https://github.com/novicezk/midjourney-proxy)接口，[接口文档](https://docs.newapi.pro/api/midjourney-proxy-image)
3. 第三方渠道[Suno API](https://github.com/Suno-API/Suno-API)接口，[接口文档](https://docs.newapi.pro/api/suno-music)
4. 自定义渠道，支持填入完整调用地址
5. Rerank模型（[Cohere](https://cohere.ai/)和[Jina](https://jina.ai/)），[接口文档](https://docs.newapi.pro/api/jinaai-rerank)
6. Claude Messages 格式，[接口文档](https://docs.newapi.pro/api/anthropic-chat)
7. Dify，当前仅支持chatflow

## 环境变量配置

详细配置说明请参考[安装指南-环境变量配置](https://docs.newapi.pro/installation/environment-variables)：

- `GENERATE_DEFAULT_TOKEN`：是否为新注册用户生成初始令牌，默认为 `false`
- `STREAMING_TIMEOUT`：流式回复超时时间，默认300秒
- `DIFY_DEBUG`：Dify渠道是否输出工作流和节点信息，默认 `true`
- `FORCE_STREAM_OPTION`：是否覆盖客户端stream_options参数，默认 `true`
- `GET_MEDIA_TOKEN`：是否统计图片token，默认 `true`
- `GET_MEDIA_TOKEN_NOT_STREAM`：非流情况下是否统计图片token，默认 `true`
- `UPDATE_TASK`：是否更新异步任务（Midjourney、Suno），默认 `true`
- `COHERE_SAFETY_SETTING`：Cohere模型安全设置，可选值为 `NONE`, `CONTEXTUAL`, `STRICT`，默认 `NONE`
- `GEMINI_VISION_MAX_IMAGE_NUM`：Gemini模型最大图片数量，默认 `16`
- `MAX_FILE_DOWNLOAD_MB`: 最大文件下载大小，单位MB，默认 `20`
- `CRYPTO_SECRET`：加密密钥，用于加密数据库内容
- `AZURE_DEFAULT_API_VERSION`：Azure渠道默认API版本，默认 `2025-04-01-preview`
- `NOTIFICATION_LIMIT_DURATION_MINUTE`：通知限制持续时间，默认 `10`分钟
- `NOTIFY_LIMIT_COUNT`：用户通知在指定持续时间内的最大数量，默认 `2`
- `ERROR_LOG_ENABLED=true`: 是否记录并显示错误日志，默认`false`

## 部署

详细部署指南请参考[安装指南-部署方式](https://docs.newapi.pro/installation)：

> [!TIP]
> 最新版Docker镜像：`bobo642/new-api:latest`  

### 多机部署注意事项
- 必须设置环境变量 `SESSION_SECRET`，否则会导致多机部署时登录状态不一致
- 如果公用Redis，必须设置 `CRYPTO_SECRET`，否则会导致多机部署时Redis内容无法获取

### 部署要求
- 本地数据库（默认）：SQLite（Docker部署必须挂载`/data`目录）
- 远程数据库：MySQL版本 >= 5.7.8，PgSQL版本 >= 9.6

### 部署方式

#### 使用宝塔面板Docker功能部署
安装宝塔面板（**9.2.0版本**及以上），在应用商店中找到**New-API**安装即可。
[图文教程](./docs/BT.md)

#### 使用Docker Compose部署（推荐）
``shell
# 下载项目
git clone https://github.com/Calcium-Ion/new-api.git
cd new-api

# 编辑 docker-compose.yml 配置
nano docker-compose.yml

# 启动服务
docker-compose up -d
```

#### 直接使用Docker镜像
``shell
# 使用SQLite
docker run --name new-api -d --restart always -p 3000:3000 -e TZ=Asia/Shanghai -v /home/ubuntu/data/new-api:/data bobo642/new-api:latest

# 使用MySQL
docker run --name new-api -d --restart always -p 3000:3000 -e SQL_DSN="root:123456@tcp(localhost:3306)/oneapi" -e TZ=Asia/Shanghai -v /home/ubuntu/data/new-api:/data bobo642/new-api:latest
```

> **💡 提示：** `-v ./data:/data` 会将数据保存在当前目录的 `data` 文件夹中，你也可以改为绝对路径如 `-v /your/custom/path:/data`

</details>

---

🎉 部署完成后，访问 `http://localhost:3000` 即可使用！

📖 更多部署方式请参考 [部署指南](https://docs.newapi.pro/installation)

---

## 📚 文档

<div align="center">

### 📖 [官方文档](https://docs.newapi.pro/) | [![Ask DeepWiki](https://deepwiki.com/badge.svg)](https://deepwiki.com/QuantumNous/new-api)

</div>

**快速导航：**

| 分类 | 链接 |
|------|------|
| 🚀 部署指南 | [安装文档](https://docs.newapi.pro/installation) |
| ⚙️ 环境配置 | [环境变量](https://docs.newapi.pro/installation/environment-variables) |
| 📡 接口文档 | [API 文档](https://docs.newapi.pro/api) |
| ❓ 常见问题 | [FAQ](https://docs.newapi.pro/support/faq) |
| 💬 社区交流 | [交流渠道](https://docs.newapi.pro/support/community-interaction) |

---

## ✨ 主要特性

> 详细特性请参考 [特性说明](https://docs.newapi.pro/wiki/features-introduction)

### 🎨 核心功能

| 特性 | 说明 |
|------|------|
| 🎨 全新 UI | 现代化的用户界面设计 |
| 🌍 多语言 | 支持中文、英文、法语、日语 |
| 🔄 数据兼容 | 完全兼容原版 One API 数据库 |
| 📈 数据看板 | 可视化控制台与统计分析 |
| 🔒 权限管理 | 令牌分组、模型限制、用户管理 |

### 💰 支付与计费

- ✅ 在线充值（易支付、Stripe）
- ✅ 模型按次数收费
- ✅ 缓存计费支持（OpenAI、Azure、DeepSeek、Claude、Qwen等所有支持的模型）
- ✅ 灵活的计费策略配置

### 🔐 授权与安全

- 😈 Discord 授权登录
- 🤖 LinuxDO 授权登录
- 📱 Telegram 授权登录
- 🔑 OIDC 统一认证
- 🔍 Key 查询使用额度（配合 [neko-api-key-tool](https://github.com/Calcium-Ion/neko-api-key-tool)）

### 🚀 高级功能

**API 格式支持：**
- ⚡ [OpenAI Responses](https://docs.newapi.pro/api/openai-responses)
- ⚡ [OpenAI Realtime API](https://docs.newapi.pro/api/openai-realtime)（含 Azure）
- ⚡ [Claude Messages](https://docs.newapi.pro/api/anthropic-chat)
- ⚡ [Google Gemini](https://docs.newapi.pro/api/google-gemini-chat/)
- 🔄 [Rerank 模型](https://docs.newapi.pro/api/jinaai-rerank)（Cohere、Jina）

**智能路由：**
- ⚖️ 渠道加权随机
- 🔄 失败自动重试
- 🚦 用户级别模型限流

**格式转换：**
- 🔄 OpenAI ⇄ Claude Messages
- 🔄 OpenAI ⇄ Gemini Chat
- 🔄 思考转内容功能

**Reasoning Effort 支持：**

<details>
<summary>查看详细配置</summary>

**OpenAI 系列模型：**
- `o3-mini-high` - High reasoning effort
- `o3-mini-medium` - Medium reasoning effort
- `o3-mini-low` - Low reasoning effort
- `gpt-5-high` - High reasoning effort
- `gpt-5-medium` - Medium reasoning effort
- `gpt-5-low` - Low reasoning effort

**Claude 思考模型：**
- `claude-3-7-sonnet-20250219-thinking` - 启用思考模式

**Google Gemini 系列模型：**
- `gemini-2.5-flash-thinking` - 启用思考模式
- `gemini-2.5-flash-nothinking` - 禁用思考模式
- `gemini-2.5-pro-thinking` - 启用思考模式
- `gemini-2.5-pro-thinking-128` - 启用思考模式，并设置思考预算为128tokens
- 也可以直接在 Gemini 模型名称后追加 `-low` / `-medium` / `-high` 来控制思考力度（无需再设置思考预算后缀）

</details>

---

## 🤖 模型支持

> 详情请参考 [接口文档 - 中继接口](https://docs.newapi.pro/api)

| 模型类型 | 说明 | 文档 |
|---------|------|------|
| 🤖 OpenAI GPTs | gpt-4-gizmo-* 系列 | - |
| 🎨 Midjourney-Proxy | [Midjourney-Proxy(Plus)](https://github.com/novicezk/midjourney-proxy) | [文档](https://docs.newapi.pro/api/midjourney-proxy-image) |
| 🎵 Suno-API | [Suno API](https://github.com/Suno-API/Suno-API) | [文档](https://docs.newapi.pro/api/suno-music) |
| 🔄 Rerank | Cohere、Jina | [文档](https://docs.newapi.pro/api/jinaai-rerank) |
| 💬 Claude | Messages 格式 | [文档](https://docs.newapi.pro/api/anthropic-chat) |
| 🌐 Gemini | Google Gemini 格式 | [文档](https://docs.newapi.pro/api/google-gemini-chat/) |
| 🔧 Dify | ChatFlow 模式 | - |
| 🎯 自定义 | 支持完整调用地址 | - |

### 📡 支持的接口

<details>
<summary>查看完整接口列表</summary>

- [聊天接口 (Chat Completions)](https://docs.newapi.pro/api/openai-chat)
- [响应接口 (Responses)](https://docs.newapi.pro/api/openai-responses)
- [图像接口 (Image)](https://docs.newapi.pro/api/openai-image)
- [音频接口 (Audio)](https://docs.newapi.pro/api/openai-audio)
- [视频接口 (Video)](https://docs.newapi.pro/api/openai-video)
- [嵌入接口 (Embeddings)](https://docs.newapi.pro/api/openai-embeddings)
- [重排序接口 (Rerank)](https://docs.newapi.pro/api/jinaai-rerank)
- [实时对话 (Realtime)](https://docs.newapi.pro/api/openai-realtime)
- [Claude 聊天](https://docs.newapi.pro/api/anthropic-chat)
- [Google Gemini 聊天](https://docs.newapi.pro/api/google-gemini-chat)

</details>

---

## 🚢 部署

> [!TIP]
> **最新版 Docker 镜像：** `calciumion/new-api:latest`

### 📋 部署要求

| 组件 | 要求 |
|------|------|
| **本地数据库** | SQLite（Docker 需挂载 `/data` 目录）|
| **远程数据库** | MySQL ≥ 5.7.8 或 PostgreSQL ≥ 9.6 |
| **容器引擎** | Docker / Docker Compose |

### ⚙️ 环境变量配置

<details>
<summary>常用环境变量配置</summary>

| 变量名 | 说明                                                           | 默认值 |
|--------|--------------------------------------------------------------|--------|
| `SESSION_SECRET` | 会话密钥（多机部署必须）                                                 | - |
| `CRYPTO_SECRET` | 加密密钥（Redis 必须）                                               | - |
| `SQL_DSN` | 数据库连接字符串                                                     | - |
| `REDIS_CONN_STRING` | Redis 连接字符串                                                  | - |
| `STREAMING_TIMEOUT` | 流式超时时间（秒）                                                    | `300` |
| `STREAM_SCANNER_MAX_BUFFER_MB` | 流式扫描器单行最大缓冲（MB），图像生成等超大 `data:` 片段（如 4K 图片 base64）需适当调大 | `64` |
| `AZURE_DEFAULT_API_VERSION` | Azure API 版本                                                 | `2025-04-01-preview` |
| `ERROR_LOG_ENABLED` | 错误日志开关                                                       | `false` |

📖 **完整配置：** [环境变量文档](https://docs.newapi.pro/installation/environment-variables)

</details>

### 🔧 部署方式

<details>
<summary><strong>方式 1：Docker Compose（推荐）</strong></summary>

```bash
# 克隆项目
git clone https://github.com/QuantumNous/new-api.git
cd new-api

# 编辑配置
nano docker-compose.yml

# 启动服务
docker-compose up -d
```

</details>

<details>
<summary><strong>方式 2：Docker 命令</strong></summary>

**使用 SQLite：**
```bash
docker run --name new-api -d --restart always \
  -p 3000:3000 \
  -e TZ=Asia/Shanghai \
  -v ./data:/data \
  calciumion/new-api:latest
```

**使用 MySQL：**
```bash
docker run --name new-api -d --restart always \
  -p 3000:3000 \
  -e SQL_DSN="root:123456@tcp(localhost:3306)/oneapi" \
  -e TZ=Asia/Shanghai \
  -v ./data:/data \
  calciumion/new-api:latest
```

> **💡 路径说明：** 
> - `./data:/data` - 相对路径，数据保存在当前目录的 data 文件夹
> - 也可使用绝对路径，如：`/your/custom/path:/data`

</details>

<details>
<summary><strong>方式 3：宝塔面板</strong></summary>

1. 安装宝塔面板（≥ 9.2.0 版本）
2. 在应用商店搜索 **New-API**
3. 一键安装

📖 [图文教程](./docs/BT.md)

</details>

### ⚠️ 多机部署注意事项

> [!WARNING]
> - **必须设置** `SESSION_SECRET` - 否则登录状态不一致
> - **公用 Redis 必须设置** `CRYPTO_SECRET` - 否则数据无法解密

### 🔄 渠道重试与缓存

**重试配置：** `设置 → 运营设置 → 通用设置 → 失败重试次数`

**缓存配置：**
- `REDIS_CONN_STRING`：Redis 缓存（推荐）
- `MEMORY_CACHE_ENABLED`：内存缓存

---

## 🔗 相关项目

### 上游项目

| 项目 | 说明 |
|------|------|
| [One API](https://github.com/songquanpeng/one-api) | 原版项目基础 |
| [Midjourney-Proxy](https://github.com/novicezk/midjourney-proxy) | Midjourney 接口支持 |

### 配套工具

| 项目 | 说明 |
|------|------|
| [neko-api-key-tool](https://github.com/Calcium-Ion/neko-api-key-tool) | Key 额度查询工具 |
| [new-api-horizon](https://github.com/Calcium-Ion/new-api-horizon) | New API 高性能优化版 |

---

## 💬 帮助支持

### 📖 文档资源

| 资源 | 链接 |
|------|------|
| 📘 常见问题 | [FAQ](https://docs.newapi.pro/support/faq) |
| 💬 社区交流 | [交流渠道](https://docs.newapi.pro/support/community-interaction) |
| 🐛 反馈问题 | [问题反馈](https://docs.newapi.pro/support/feedback-issues) |
| 📚 完整文档 | [官方文档](https://docs.newapi.pro/support) |

### 🤝 贡献指南

欢迎各种形式的贡献！

- 🐛 报告 Bug
- 💡 提出新功能
- 📝 改进文档
- 🔧 提交代码

---

## 🌟 Star History

<div align="center">

[![Star History Chart](https://api.star-history.com/svg?repos=Calcium-Ion/new-api&type=Date)](https://star-history.com/#Calcium-Ion/new-api&Date)

</div>

---

<div align="center">

### 💖 感谢使用 New API

如果这个项目对你有帮助，欢迎给我们一个 ⭐️ Star！

**[官方文档](https://docs.newapi.pro/)** • **[问题反馈](https://github.com/Calcium-Ion/new-api/issues)** • **[最新发布](https://github.com/Calcium-Ion/new-api/releases)**

<sub>Built with ❤️ by QuantumNous</sub>

</div>
