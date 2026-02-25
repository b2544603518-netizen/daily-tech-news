# 研发数字化每日资讯 | R&D Digitalization Daily News

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live-brightgreen)](https://b2544603518-netizen.github.io/daily-tech-news/)
[![Update Script](https://img.shields.io/badge/Update-Python%20Script-blue)](update_daily_news.py)
[![Last Updated](https://img.shields.io/badge/Last%20Updated-2026--02--25-orange)](https://b2544603518-netizen.github.io/daily-tech-news/)

## 📋 项目简介 | Project Overview

### 中文
本项目是一个**研发数字化行业每日资讯聚合站点**，专注于收集和整理ALM/PLM、研发数字化、机器人、无人机、低空经济、智能制造等领域的前沿动态。所有资讯均来自权威媒体，附带原文链接，确保信息真实可信。

**覆盖领域：**
- 🚁 低空经济 · 无人机（eVTOL、政策动态、市场格局）
- 🤖 机器人 · 具身智能（人形机器人、四足机器人、产业应用）
- 💻 研发数字化 · PLM/ALM（产品生命周期管理、应用生命周期管理）
- 🏭 智能制造 · 数字化转型（工业互联网、示范工厂、信创适配）
- 🚐 无人配送车（九识智能、新石器、白犀牛等）
- 🛵 两轮车 · 电动车（雅迪、小牛、九号公司、共享单车）
- 🔋 共享充电宝（怪兽充电、小电科技、美团充电宝）

**固定网址：** https://b2544603518-netizen.github.io/daily-tech-news/

### English
This project is a **daily news aggregation site for R&D digitalization**, focusing on collecting and curating cutting-edge developments in ALM/PLM, R&D digitalization, robotics, drones, low-altitude economy, and intelligent manufacturing. All news is sourced from authoritative media with original links to ensure credibility.

**Coverage Areas:**
- 🚁 Low-Altitude Economy · Drones (eVTOL, policy dynamics, market landscape)
- 🤖 Robotics · Embodied AI (Humanoid robots, quadruped robots, industrial applications)
- 💻 R&D Digitalization · PLM/ALM (Product Lifecycle Management, Application Lifecycle Management)
- 🏭 Intelligent Manufacturing · Digital Transformation (Industrial Internet, demonstration factories, localization adaptation)
- 🚐 Autonomous Delivery Vehicles (Jiushi Intelligence, Neolix, White Rhino, etc.)
- 🛵 Two-wheelers · Electric Vehicles (Yadea, NIU, Ninebot, bike-sharing)
- 🔋 Shared Power Banks (Energy Monster, Xiaodian Technology, Meituan Power Bank)

**Permanent URL:** https://b2544603518-netizen.github.io/daily-tech-news/

---

## 🗂️ 文件结构 | File Structure

```
gemini 测试/
├── README.md                           # 项目说明文档
├── update_daily_news.py                # 自动部署脚本
├── 研发数字化每日资讯_2026-02-25.html  # 每日资讯页面（示例）
└── 每日资讯更新Prompt.md               # 更新任务Prompt模板
```

**GitHub Pages 部署结构：**
```
daily-tech-news/
├── index.html              # 最新一期（固定入口）
├── 2026-02-25.html         # 历史归档
├── 2026-02-26.html         # 历史归档
├── dates.json              # 日期索引（供前端导航）
└── ...
```

---

## 🚀 快速开始 | Quick Start

### 本地预览 | Local Preview

```bash
# 克隆仓库（如果有）
git clone <repository-url>

# 直接在浏览器中打开HTML文件
open 研发数字化每日资讯_2026-02-25.html
```

### 部署新资讯 | Deploy New Edition

```bash
# 使用部署脚本推送至GitHub Pages
python3 update_daily_news.py "研发数字化每日资讯_YYYY-MM-DD.html"
```

**脚本功能：**
1. 上传指定HTML文件为日期归档（如 `2026-02-25.html`）
2. 更新 `index.html` 为最新入口
3. 更新 `dates.json` 日期索引

---

## 📰 内容规范 | Content Guidelines

### 收录标准 | Inclusion Criteria

1. **真实来源**：所有资讯必须来自权威媒体（新华网、央视网、光明网、经济观察网、腾讯新闻、新浪财经、虎嗅网、IT之家等）
2. **原文链接**：每条资讯必须附带可点击的原文链接
3. **今日新增**：标注发布时间，区分"今日新增"与往期内容
4. **标签分类**：使用标签系统（低空经济、人形机器人、PLM、ALM等）

### 内容格式 | Content Format

```html
<div class="news-item">
  <div class="title">新闻标题</div>
  <div class="source">来源：媒体名称 · 发布时间</div>
  <div class="tags">
    <span class="hot">今日新增</span>
    <span>标签1</span>
    <span>标签2</span>
  </div>
  <div class="desc">新闻摘要...</div>
  <div class="link"><a href="原文链接" target="_blank">🔗 查看原文</a></div>
</div>
```

---

## 🛠️ 技术实现 | Technical Implementation

### 前端技术 | Frontend
- **纯HTML/CSS**：无需构建工具，直接部署
- **响应式设计**：适配桌面端和移动端
- **日期导航**：Sticky顶部导航栏，支持日期切换
- **动态加载**：JavaScript动态加载 `dates.json` 生成导航

### 部署技术 | Deployment
- **GitHub Pages**：静态网站托管
- **GitHub API**：通过Python脚本自动推送文件
- **Base64编码**：通过GitHub Contents API更新文件

---

## 📊 数据源 | Data Sources

### 权威媒体 | Authoritative Media
- **官方媒体**：新华网、央视网、光明网、人民网
- **财经媒体**：经济观察网、新浪财经、东方财富、21经济网
- **科技媒体**：虎嗅网、IT之家、36氪、晚点LatePost
- **行业媒体**：OFweek、智东西、赛迪网

### 企业官方 | Official Sources
- PTC官方、西门子官网、达索系统官网
- 宇树科技、大疆创新、亿航智能
- 雅迪、小牛电动、九号公司

---

## 🤝 贡献指南 | Contribution Guide

### 如何添加新资讯 | How to Add News

1. **准备HTML文件**：按照模板格式创建每日资讯
2. **本地验证**：在浏览器中预览确保格式正确
3. **运行部署**：执行 `update_daily_news.py` 脚本
4. **检查上线**：访问GitHub Pages确认部署成功

### 模板预留板块 | Template Reserved Sections

新添加的行业板块使用预留格式：

```html
<div class="news-item">
  <div class="title">【板块预留】板块名称</div>
  <div class="source">待补充：具体数据来源</div>
  <div class="tags"><span>标签</span></div>
  <div class="desc">本板块将收录...（列出预计收录内容）</div>
</div>
```

---

## 📜 更新历史 | Update History

| 日期 | 更新内容 | 操作者 |
|------|---------|--------|
| 2026-02-25 | 初始化项目，添加低空经济、机器人、PLM/ALM、智能制造板块 | CatPaw AI |
| 2026-02-25 | 新增无人配送车、两轮车（含电动车）、共享充电宝板块结构 | CatPaw AI |

---

## ⚠️ 免责声明 | Disclaimer

1. **内容来源**：所有资讯内容均来源于网络公开信息，版权归原作者所有
2. **准确性**：我们尽力确保信息准确，但不保证内容的绝对正确性
3. **时效性**：资讯具有时效性，请以原文发布时间和内容为准
4. **投资建议**：本资讯仅供参考，不构成任何投资建议

---

## 📧 联系方式 | Contact

- **项目主页**：https://b2544603518-netizen.github.io/daily-tech-news/
- **GitHub仓库**：https://github.com/b2544603518-netizen/daily-tech-news
- **问题反馈**：通过GitHub Issues提交

---

## 📝 License

本项目采用 MIT License 开源协议。

---

<p align="center">
  <sub>Built with ❤️ by CatPaw AI · 2026</sub>
</p>
