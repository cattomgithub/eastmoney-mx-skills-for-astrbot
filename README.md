# 东方财富妙想 Skills (AstrBot 版)

本仓库基于[东方财富官方 Skills ](https://marketing.dfcfs.com/views/finskillshub/index)修改，包含 5 个可直接用于 AstrBot 的独立 Skill 目录：

- `mx-data`：妙想金融数据 skill
- `mx-search`：妙想资讯搜索 skill
- `mx-xuangu`：妙想智能选股 skill
- `mx-zixuan`：妙想自选股管理 skill
- `mx-moni`：妙想模拟组合管理 skill

每个目录都包含 `SKILL.md` 与对应 Python 脚本，可单独打包上传到 AstrBot。

## 运行依赖

- Python 3.10+
- `requests` `pandas` `openpyxl`

## 环境变量

- `MX_APIKEY` (必填): 妙想技能 API Key
- `MX_API_URL` (可选，仅 `mx-moni` 使用): 默认为 `https://mkapi2.dfcfs.com/finskillshub`
- `MX_OUTPUT_DIR` (可惜): 覆盖输出目录 (默认 `./output/`)

## 与官方版本的差异

- 去除了 OpenClaw/ClawHub 的安装路径说明
- 默认输出目录统一为 Skill 目录下的 `./output/`
- 支持通过环境变量 `MX_OUTPUT_DIR` 覆盖默认输出目录
