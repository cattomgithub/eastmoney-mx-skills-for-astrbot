# 东方财富妙想 Skills

本仓库基于[东方财富官方 Skills](https://marketing.dfcfs.com/views/finskillshub/index)，参考 [Anthropic Agent Skills](https://agentskills.io/home) 规范修改，包含 5 个独立 Skill 目录：

- `mx-data`：妙想金融数据 skill *已验证可用*
- `mx-search`：妙想资讯搜索 skill *已验证可用*
- `mx-xuangu`：妙想智能选股 skill *已验证可用*
- `mx-zixuan`：妙想自选股管理 skill
- `mx-moni`：妙想模拟组合管理 skill

每个目录都包含 `SKILL.md` 与对应 Python 脚本。**每个 Skills 对应的 Zip 压缩包已打包在 [Release](https://github.com/cattomgithub/eastmoney-mx-skills-for-astrbot/releases/latest)。**

## 运行依赖

- Python 3.10+
- `requests` `pandas` `openpyxl`

## 环境变量

- `MX_APIKEY` (必填): 妙想技能 API Key
- `MX_API_URL` (可选，仅 `mx-moni` 使用): 默认为 `https://mkapi2.dfcfs.com/finskillshub`
- `MX_OUTPUT_DIR` (可选): 覆盖输出目录 (默认 `./output/`)
