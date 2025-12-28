<p align="right">
   <a href="./README.md">中文</a> | <strong>English</strong>
</p>
<div align="center">

![new-api](/web/public/logo.png)

# New API

🍥 Next-Generation Large Model Gateway and AI Asset Management System

<a href="https://trendshift.io/repositories/8227" target="_blank"><img src="https://trendshift.io/api/badge/repositories/8227" alt="Calcium-Ion%2Fnew-api | Trendshift" style="width: 250px; height: 55px;" width="250" height="55"/></a>

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
</div>

## 📝 Project Description

> [!NOTE]
> This is an open-source project developed based on [One API](https://github.com/songquanpeng/one-api)

> [!IMPORTANT]
> - This project is for personal learning purposes only, with no guarantee of stability or technical support.
> - Users must comply with OpenAI's [Terms of Use](https://openai.com/policies/terms-of-use) and **applicable laws and regulations**, and must not use it for illegal purposes.
> - According to the [《Interim Measures for the Management of Generative Artificial Intelligence Services》](http://www.cac.gov.cn/2023-07/13/c_1690898327029107.htm), please do not provide any unregistered generative AI services to the public in China.

<h2>🤝 Trusted Partners</h2>
<p id="premium-sponsors">&nbsp;</p>
<p align="center"><strong>No particular order</strong></p>
<p align="center">
  <a href="https://www.cherry-ai.com/" target=_blank><img
    src="./docs/images/cherry-studio.png" alt="Cherry Studio" height="120"
  /></a>
  <a href="https://bda.pku.edu.cn/" target=_blank><img
    src="./docs/images/pku.png" alt="Peking University" height="120"
  /></a>
  <a href="https://www.compshare.cn/?ytag=GPU_yy_gh_newapi" target=_blank><img
    src="./docs/images/ucloud.png" alt="UCloud" height="120"
  /></a>
  <a href="https://www.aliyun.com/" target=_blank><img
    src="./docs/images/aliyun.png" alt="Alibaba Cloud" height="120"
  /></a>
  <a href="https://io.net/" target=_blank><img
    src="./docs/images/io-net.png" alt="IO.NET" height="120"
  /></a>
</p>
<<<<<<< HEAD
<p>&nbsp;</p>
=======

<p align="center">
  <a href="https://www.cherry-ai.com/" target="_blank">
    <img src="./docs/images/cherry-studio.png" alt="Cherry Studio" height="80" />
  </a>
  <a href="https://bda.pku.edu.cn/" target="_blank">
    <img src="./docs/images/pku.png" alt="Peking University" height="80" />
  </a>
  <a href="https://www.compshare.cn/?ytag=GPU_yy_gh_newapi" target="_blank">
    <img src="./docs/images/ucloud.png" alt="UCloud" height="80" />
  </a>
  <a href="https://www.aliyun.com/" target="_blank">
    <img src="./docs/images/aliyun.png" alt="Alibaba Cloud" height="80" />
  </a>
  <a href="https://io.net/" target="_blank">
    <img src="./docs/images/io-net.png" alt="IO.NET" height="80" />
  </a>
</p>

---

## 🙏 Special Thanks

<p align="center">
  <a href="https://www.jetbrains.com/?from=new-api" target="_blank">
    <img src="https://resources.jetbrains.com/storage/products/company/brand/logos/jb_beam.png" alt="JetBrains Logo" width="120" />
  </a>
</p>

<p align="center">
  <strong>Thanks to <a href="https://www.jetbrains.com/?from=new-api">JetBrains</a> for providing free open-source development license for this project</strong>
</p>

---

## 🚀 Quick Start

### Using Docker Compose (Recommended)

```bash
# Clone the project
git clone https://github.com/QuantumNous/new-api.git
cd new-api

# Edit docker-compose.yml configuration
nano docker-compose.yml

# Start the service
docker-compose up -d
```

<details>
<summary><strong>Using Docker Commands</strong></summary>

```bash
# Pull the latest image
docker pull calciumion/new-api:latest

# Using SQLite (default)
docker run --name new-api -d --restart always \
  -p 3000:3000 \
  -e TZ=Asia/Shanghai \
  -v ./data:/data \
  calciumion/new-api:latest

# Using MySQL
docker run --name new-api -d --restart always \
  -p 3000:3000 \
  -e SQL_DSN="root:123456@tcp(localhost:3306)/oneapi" \
  -e TZ=Asia/Shanghai \
  -v ./data:/data \
  calciumion/new-api:latest
```

> **💡 Tip:** `-v ./data:/data` will save data in the `data` folder of the current directory, you can also change it to an absolute path like `-v /your/custom/path:/data`

</details>

---

🎉 After deployment is complete, visit `http://localhost:3000` to start using!

📖 For more deployment methods, please refer to [Deployment Guide](https://docs.newapi.pro/en/docs/installation)

---
>>>>>>> upstream/main

## 📚 Documentation

For detailed documentation, please visit our official Wiki: [https://docs.newapi.pro/](https://docs.newapi.pro/)

<<<<<<< HEAD
You can also access the AI-generated DeepWiki:
[![Ask DeepWiki](https://deepwiki.com/badge.svg)](https://deepwiki.com/QuantumNous/new-api)

## ✨ Key Features

New API offers a wide range of features, please refer to [Features Introduction](https://docs.newapi.pro/wiki/features-introduction) for details:
=======
### 📖 [Official Documentation](https://docs.newapi.pro/en/docs) | [![Ask DeepWiki](https://deepwiki.com/badge.svg)](https://deepwiki.com/QuantumNous/new-api)

</div>

**Quick Navigation:**

| Category | Link |
|------|------|
| 🚀 Deployment Guide | [Installation Documentation](https://docs.newapi.pro/en/docs/installation) |
| ⚙️ Environment Configuration | [Environment Variables](https://docs.newapi.pro/en/docs/installation/config-maintenance/environment-variables) |
| 📡 API Documentation | [API Documentation](https://docs.newapi.pro/en/docs/api) |
| ❓ FAQ | [FAQ](https://docs.newapi.pro/en/docs/support/faq) |
| 💬 Community Interaction | [Communication Channels](https://docs.newapi.pro/en/docs/support/community-interaction) |

---

## ✨ Key Features

> For detailed features, please refer to [Features Introduction](https://docs.newapi.pro/en/docs/guide/wiki/basic-concepts/features-introduction)
>>>>>>> upstream/main

1. 🎨 Brand new UI interface
2. 🌍 Multi-language support
3. 💰 Online recharge functionality (YiPay)
4. 🔍 Support for querying usage quotas with keys (works with [neko-api-key-tool](https://github.com/Calcium-Ion/neko-api-key-tool))
5. 🔄 Compatible with the original One API database
6. 💵 Support for pay-per-use model pricing
7. ⚖️ Support for weighted random channel selection
8. 📈 Data dashboard (console)
9. 🔒 Token grouping and model restrictions
10. 🤖 Support for more authorization login methods (LinuxDO, Telegram, OIDC)
11. 🔄 Support for Rerank models (Cohere and Jina), [API Documentation](https://docs.newapi.pro/api/jinaai-rerank)
12. ⚡ Support for OpenAI Realtime API (including Azure channels), [API Documentation](https://docs.newapi.pro/api/openai-realtime)
13. ⚡ Support for Claude Messages format, [API Documentation](https://docs.newapi.pro/api/anthropic-chat)
14. Support for entering chat interface via /chat2link route
15. 🧠 Support for setting reasoning effort through model name suffixes:
    1. OpenAI o-series models
     - Add `-high` suffix for high reasoning effort (e.g.: `o3-mini-high`)
     - Add `-medium` suffix for medium reasoning effort (e.g.: `o3-mini-medium`)
     - Add `-low` suffix for low reasoning effort (e.g.: `o3-mini-low`)
    2. Claude thinking models
     - Add `-thinking` suffix to enable thinking mode (e.g.: `claude-3-7-sonnet-20250219-thinking`)
16. 🔄 Thinking-to-content functionality
17. 🔄 Model rate limiting for users
18. 💰 Cache billing support, which allows billing at a set ratio when cache is hit:
    1. Set the `Prompt Cache Ratio` option in `System Settings-Operation Settings`
    2. Set `Prompt Cache Ratio` in the channel, range 0-1, e.g., setting to 0.5 means billing at 50%
    when cache is hit
    3. Supported channels:
     - [x] OpenAI
     - [x] Azure
     - [x] DeepSeek
     - [x] Claude

## Model Support

This version supports multiple models, please refer to [API Documentation-Relay Interface](https://docs.newapi.pro/api) for details:

1. Third-party models **gpts** (gpt-4-gizmo-*)
2. Third-party channel [Midjourney-Proxy(Plus)](https://github.com/novicezk/midjourney-proxy) interface, [API Documentation](https://docs.newapi.pro/api/midjourney-proxy-image)
3. Third-party channel [Suno API](https://github.com/Suno-API/Suno-API) interface, [API Documentation](https://docs.newapi.pro/api/suno-music)
4. Custom channels, supporting full call address input
5. Rerank models ([Cohere](https://cohere.ai/) and [Jina](https://jina.ai/)), [API Documentation](https://docs.newapi.pro/api/jinaai-rerank)
6. Claude Messages format, [API Documentation](https://docs.newapi.pro/api/anthropic-chat)
7. Dify, currently only supports chatflow

## Environment Variable Configuration

For detailed configuration instructions, please refer to [Installation Guide-Environment Variables Configuration](https://docs.newapi.pro/installation/environment-variables):

- `GENERATE_DEFAULT_TOKEN`: Whether to generate initial tokens for newly registered users, default is `false`
- `STREAMING_TIMEOUT`: Streaming response timeout, default is 300 seconds
- `DIFY_DEBUG`: Whether to output workflow and node information for Dify channels, default is `true`
- `FORCE_STREAM_OPTION`: Whether to override client stream_options parameter, default is `true`
- `GET_MEDIA_TOKEN`: Whether to count image tokens, default is `true`
- `GET_MEDIA_TOKEN_NOT_STREAM`: Whether to count image tokens in non-streaming cases, default is `true`
- `UPDATE_TASK`: Whether to update asynchronous tasks (Midjourney, Suno), default is `true`
- `COHERE_SAFETY_SETTING`: Cohere model safety settings, options are `NONE`, `CONTEXTUAL`, `STRICT`, default is `NONE`
- `GEMINI_VISION_MAX_IMAGE_NUM`: Maximum number of images for Gemini models, default is `16`
- `MAX_FILE_DOWNLOAD_MB`: Maximum file download size in MB, default is `20`
- `CRYPTO_SECRET`: Encryption key used for encrypting database content
- `AZURE_DEFAULT_API_VERSION`: Azure channel default API version, default is `2025-04-01-preview`
- `NOTIFICATION_LIMIT_DURATION_MINUTE`: Notification limit duration, default is `10` minutes
- `NOTIFY_LIMIT_COUNT`: Maximum number of user notifications within the specified duration, default is `2`
- `ERROR_LOG_ENABLED=true`: Whether to record and display error logs, default is `false`

<<<<<<< HEAD
## Deployment

For detailed deployment guides, please refer to [Installation Guide-Deployment Methods](https://docs.newapi.pro/installation):
=======
**API Format Support:**
- ⚡ [OpenAI Responses](https://docs.newapi.pro/en/docs/api/ai-model/chat/openai/create-response)
- ⚡ [OpenAI Realtime API](https://docs.newapi.pro/en/docs/api/ai-model/realtime/create-realtime-session) (including Azure)
- ⚡ [Claude Messages](https://docs.newapi.pro/en/docs/api/ai-model/chat/create-message)
- ⚡ [Google Gemini](https://doc.newapi.pro/en/api/google-gemini-chat)
- 🔄 [Rerank Models](https://docs.newapi.pro/en/docs/api/ai-model/rerank/create-rerank) (Cohere, Jina)

**Intelligent Routing:**
- ⚖️ Channel weighted random
- 🔄 Automatic retry on failure
- 🚦 User-level model rate limiting

**Format Conversion:**
- 🔄 OpenAI ⇄ Claude Messages
- 🔄 OpenAI ⇄ Gemini Chat
- 🔄 Thinking-to-content functionality

**Reasoning Effort Support:**

<details>
<summary>View detailed configuration</summary>

**OpenAI series models:**
- `o3-mini-high` - High reasoning effort
- `o3-mini-medium` - Medium reasoning effort
- `o3-mini-low` - Low reasoning effort
- `gpt-5-high` - High reasoning effort
- `gpt-5-medium` - Medium reasoning effort
- `gpt-5-low` - Low reasoning effort

**Claude thinking models:**
- `claude-3-7-sonnet-20250219-thinking` - Enable thinking mode

**Google Gemini series models:**
- `gemini-2.5-flash-thinking` - Enable thinking mode
- `gemini-2.5-flash-nothinking` - Disable thinking mode
- `gemini-2.5-pro-thinking` - Enable thinking mode
- `gemini-2.5-pro-thinking-128` - Enable thinking mode with thinking budget of 128 tokens
- You can also append `-low`, `-medium`, or `-high` to any Gemini model name to request the corresponding reasoning effort (no extra thinking-budget suffix needed).

</details>

---

## 🤖 Model Support

> For details, please refer to [API Documentation - Relay Interface](https://docs.newapi.pro/en/docs/api)

| Model Type | Description | Documentation |
|---------|------|------|
| 🤖 OpenAI GPTs | gpt-4-gizmo-* series | - |
| 🎨 Midjourney-Proxy | [Midjourney-Proxy(Plus)](https://github.com/novicezk/midjourney-proxy) | [Documentation](https://doc.newapi.pro/en/api/midjourney-proxy-image) |
| 🎵 Suno-API | [Suno API](https://github.com/Suno-API/Suno-API) | [Documentation](https://doc.newapi.pro/en/api/suno-music) |
| 🔄 Rerank | Cohere, Jina | [Documentation](https://docs.newapi.pro/en/docs/api/ai-model/rerank/create-rerank) |
| 💬 Claude | Messages format | [Documentation](https://docs.newapi.pro/en/docs/api/ai-model/chat/create-message) |
| 🌐 Gemini | Google Gemini format | [Documentation](https://doc.newapi.pro/en/api/google-gemini-chat) |
| 🔧 Dify | ChatFlow mode | - |
| 🎯 Custom | Supports complete call address | - |

### 📡 Supported Interfaces

<details>
<summary>View complete interface list</summary>

- [Chat Interface (Chat Completions)](https://docs.newapi.pro/en/docs/api/ai-model/chat/openai/create-chat-completion)
- [Response Interface (Responses)](https://docs.newapi.pro/en/docs/api/ai-model/chat/openai/create-response)
- [Image Interface (Image)](https://docs.newapi.pro/en/docs/api/ai-model/images/openai/v1-images-generations--post)
- [Audio Interface (Audio)](https://docs.newapi.pro/en/docs/api/ai-model/audio/openai/create-transcription)
- [Video Interface (Video)](https://docs.newapi.pro/en/docs/api/ai-model/videos/create-video-generation)
- [Embedding Interface (Embeddings)](https://docs.newapi.pro/en/docs/api/ai-model/embeddings/create-embedding)
- [Rerank Interface (Rerank)](https://docs.newapi.pro/en/docs/api/ai-model/rerank/create-rerank)
- [Realtime Conversation (Realtime)](https://docs.newapi.pro/en/docs/api/ai-model/realtime/create-realtime-session)
- [Claude Chat](https://docs.newapi.pro/en/docs/api/ai-model/chat/create-message)
- [Google Gemini Chat](https://doc.newapi.pro/en/api/google-gemini-chat)

</details>

---

## 🚢 Deployment
>>>>>>> upstream/main

> [!TIP]
> Latest Docker image: `bobo642/new-api:latest`

### Multi-machine Deployment Considerations
- Environment variable `SESSION_SECRET` must be set, otherwise login status will be inconsistent across multiple machines
- If sharing Redis, `CRYPTO_SECRET` must be set, otherwise Redis content cannot be accessed across multiple machines

### Deployment Requirements
- Local database (default): SQLite (Docker deployment must mount the `/data` directory)
- Remote database: MySQL version >= 5.7.8, PgSQL version >= 9.6

### Deployment Methods

#### Using BaoTa Panel Docker Feature
Install BaoTa Panel (version **9.2.0** or above), find **New-API** in the application store and install it.
[Tutorial with images](./docs/BT.md)

<<<<<<< HEAD
#### Using Docker Compose (Recommended)
``shell
# Download the project
git clone https://github.com/Calcium-Ion/new-api.git
=======
| Variable Name | Description | Default Value |
|--------|------|--------|
| `SESSION_SECRET` | Session secret (required for multi-machine deployment) | - |
| `CRYPTO_SECRET` | Encryption secret (required for Redis) | - |
| `SQL_DSN` | Database connection string | - |
| `REDIS_CONN_STRING` | Redis connection string | - |
| `STREAMING_TIMEOUT` | Streaming timeout (seconds) | `300` |
| `STREAM_SCANNER_MAX_BUFFER_MB` | Max per-line buffer (MB) for the stream scanner; increase when upstream sends huge image/base64 payloads | `64` |
| `MAX_REQUEST_BODY_MB` | Max request body size (MB, counted **after decompression**; prevents huge requests/zip bombs from exhausting memory). Exceeding it returns `413` | `32` |
| `AZURE_DEFAULT_API_VERSION` | Azure API version | `2025-04-01-preview` |
| `ERROR_LOG_ENABLED` | Error log switch | `false` |
| `PYROSCOPE_URL` | Pyroscope server address | - |
| `PYROSCOPE_APP_NAME` | Pyroscope application name | `new-api` |
| `PYROSCOPE_BASIC_AUTH_USER` | Pyroscope basic auth user | - |
| `PYROSCOPE_BASIC_AUTH_PASSWORD` | Pyroscope basic auth password | - |
| `PYROSCOPE_MUTEX_RATE` | Pyroscope mutex sampling rate | `5` |
| `PYROSCOPE_BLOCK_RATE` | Pyroscope block sampling rate | `5` |
| `HOSTNAME` | Hostname tag for Pyroscope | `new-api` |

📖 **Complete configuration:** [Environment Variables Documentation](https://docs.newapi.pro/en/docs/installation/config-maintenance/environment-variables)

</details>

### 🔧 Deployment Methods

<details>
<summary><strong>Method 1: Docker Compose (Recommended)</strong></summary>

```bash
# Clone the project
git clone https://github.com/QuantumNous/new-api.git
>>>>>>> upstream/main
cd new-api
# Edit docker-compose.yml as needed
# Start
docker-compose up -d
```

#### Using Docker Image Directly
``shell
# Using SQLite
docker run --name new-api -d --restart always -p 3000:3000 -e TZ=Asia/Shanghai -v /home/ubuntu/data/new-api:/data bobo642/new-api:latest

# Using MySQL
docker run --name new-api -d --restart always -p 3000:3000 -e SQL_DSN="root:123456@tcp(localhost:3306)/oneapi" -e TZ=Asia/Shanghai -v /home/ubuntu/data/new-api:/data bobo642/new-api:latest
```

## Channel Retry and Cache
Channel retry functionality has been implemented, you can set the number of retries in
`Settings->Operation Settings->General Settings`. It is **recommended to enable caching**.

### Cache Configuration Method
1. `REDIS_CONN_STRING`: Set Redis as cache
2. `MEMORY_CACHE_ENABLED`: Enable memory cache (no need to set manually if Redis is set)

## API Documentation

For detailed API documentation, please refer to [API Documentation](https://docs.newapi.pro/api):

- [Chat API](https://docs.newapi.pro/api/openai-chat)
- [Image API](https://docs.newapi.pro/api/openai-image)
- [Rerank API](https://docs.newapi.pro/api/jinaai-rerank)
- [Realtime API](https://docs.newapi.pro/api/openai-realtime)
- [Claude Chat API (messages)](https://docs.newapi.pro/api/anthropic-chat)

## Related Projects
- [One API](https://github.com/songquanpeng/one-api): Original project
- [Midjourney-Proxy](https://github.com/novicezk/midjourney-proxy): Midjourney interface support
- [chatnio](https://github.com/Deeptrain-Community/chatnio): Next-generation AI one-stop B/C-end solution
- [neko-api-key-tool](https://github.com/Calcium-Ion/neko-api-key-tool): Query usage quota with key

Other projects based on New API:
- [new-api-horizon](https://github.com/Calcium-Ion/new-api-horizon): High-performance optimized version of New API
- [VoAPI](https://github.com/VoAPI/VoAPI): Frontend beautified version based on New API

## Help and Support

<<<<<<< HEAD
If you have any questions, please refer to [Help and Support](https://docs.newapi.pro/support):
- [Community Interaction](https://docs.newapi.pro/support/community-interaction)
- [Issue Feedback](https://docs.newapi.pro/support/feedback-issues)
- [FAQ](https://docs.newapi.pro/support/faq)
=======
> [!WARNING]
> - **Must set** `SESSION_SECRET` - Otherwise login status inconsistent
> - **Shared Redis must set** `CRYPTO_SECRET` - Otherwise data cannot be decrypted

### 🔄 Channel Retry and Cache

**Retry configuration:** `Settings → Operation Settings → General Settings → Failure Retry Count`

**Cache configuration:**
- `REDIS_CONN_STRING`: Redis cache (recommended)
- `MEMORY_CACHE_ENABLED`: Memory cache

---

## 🔗 Related Projects

### Upstream Projects

| Project | Description |
|------|------|
| [One API](https://github.com/songquanpeng/one-api) | Original project base |
| [Midjourney-Proxy](https://github.com/novicezk/midjourney-proxy) | Midjourney interface support |

### Supporting Tools

| Project | Description |
|------|------|
| [neko-api-key-tool](https://github.com/Calcium-Ion/neko-api-key-tool) | Key quota query tool |
| [new-api-horizon](https://github.com/Calcium-Ion/new-api-horizon) | New API high-performance optimized version |

---

## 💬 Help Support

### 📖 Documentation Resources

| Resource | Link |
|------|------|
| 📘 FAQ | [FAQ](https://docs.newapi.pro/en/docs/support/faq) |
| 💬 Community Interaction | [Communication Channels](https://docs.newapi.pro/en/docs/support/community-interaction) |
| 🐛 Issue Feedback | [Issue Feedback](https://docs.newapi.pro/en/docs/support/feedback-issues) |
| 📚 Complete Documentation | [Official Documentation](https://docs.newapi.pro/en/docs) |

### 🤝 Contribution Guide

Welcome all forms of contribution!

- 🐛 Report Bugs
- 💡 Propose New Features
- 📝 Improve Documentation
- 🔧 Submit Code

---
>>>>>>> upstream/main

## 🌟 Star History

[![Star History Chart](https://api.star-history.com/svg?repos=Calcium-Ion/new-api&type=Date)](https://star-history.com/#Calcium-Ion/new-api&Date)
<<<<<<< HEAD
=======

</div>

---

<div align="center">

### 💖 Thank you for using New API

If this project is helpful to you, welcome to give us a ⭐️ Star！

**[Official Documentation](https://docs.newapi.pro/en/docs)** • **[Issue Feedback](https://github.com/Calcium-Ion/new-api/issues)** • **[Latest Release](https://github.com/Calcium-Ion/new-api/releases)**

<sub>Built with ❤️ by QuantumNous</sub>

</div>
>>>>>>> upstream/main
