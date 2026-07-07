# TTCS - AI 声音克隆与配音工具

![TTCS V0.4.2](https://img.shields.io/badge/Version-0.4.2-brightgreen)
![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![License](https://img.shields.io/badge/License-MIT-purple)

**TTCS (Text To Cloned Speech)** 是一款强大的开源文字转语音与 AI 声音克隆工具。它将复杂的语音合成技术提纯，为您提供“开箱即用”的桌面级体验。

## ✨ 核心亮点

- **⚡ 极速声音复刻**：仅需一段 5-10 秒的纯净音频，即可完美克隆出目标声音的音色。
- **🎙️ 纯净文本配音**：内置全量 16kHz PCM 引擎，提供极其纯净、自然的文字配音。
- **👩‍🦰 预置经典音色**：内置 3 男 3 女高拟真经典音色，满足多种创作需求。
- **🛡️ 极致容错架构 (V0.4.2 专属)**：全面修复音频转码假死 Bug，无论传入何种格式音频，都能智能清洗并稳定输出。
- **💻 解压即用**：无需繁琐的 Python 环境配置，小白也可直接通过 Release 包一键运行。

## 🚀 快速上手 (针对普通用户)

如果您只想快速体验，不想折腾环境：
1. 请前往本项目的 [**Releases 页面**](https://github.com/qq85182147-arch/ttcs/releases)
2. 下载最新版本（如 `TTCS_V0.4.2_Release.zip`，体积约 1.85GB）。
3. 解压到本地，双击 `run_TTCS.bat` 即可直接运行。

## 🛠️ 开发者指南 (针对极客与开发者)

如果您希望参与二次开发或自行打包：
1. **克隆代码**：下载本仓库的源码压缩包或执行 `git clone`。
2. **安装依赖**：建议使用虚拟环境，并执行 `pip install -r requirements.txt` (请根据您的显卡配置 PyTorch)。
3. **补充模型文件**：运行源码需要补充模型库，具体路径结构请参考代码内的模型加载逻辑。
4. **运行源码**：执行 `python src/app_main.py` 启动图形界面。

## 📝 更新日志

**V0.4.2 **
- 优化 ASR (语音识别) 流程，强制统一音频输入格式至 16kHz 单声道纯种 WAV。
- 解决极端格式音频导致的隐蔽假死现象。
- 增加容错报错提示，极大提升工作流的稳定性。
