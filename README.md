# 📚 TMUA Practice

TMUA（Test of Mathematics for University Admission）在线练习系统，纯前端实现，无需服务器。

## ✨ 功能

### 学生端（index.html）

- **280 道真题** — 覆盖 2016–2022 年 Paper 1 & Paper 2
- **年份/试卷筛选** — 按年份和 Paper 快速定位题目
- **答题卡侧边栏** — 按年份 → Paper 分组，可折叠，点击跳转
- **模拟考试** — 选定试卷后限时 75 分钟，交卷出成绩
- **随机练习** — Fisher-Yates 洗牌打乱题目顺序
- **错题二刷** — 一键重做所有做错的题
- **知识点诊断** — 按知识点统计正确率，定位薄弱环节
- **暗黑模式** — 护眼主题，自动记忆偏好
- **图形题支持** — 19 道含图题目，KaTeX 数学公式渲染
- **进度自动保存** — 基于 localStorage，关闭页面不丢数据
- **成绩提交** — 模考结束后可一键提交成绩给老师 ⭐新增

### 教师端（dashboard.html）

- **实时数据看板** — 自动拉取学生成绩数据 ⭐新增
- **统计概览** — 总提交数、平均正确率、今日提交、最高分
- **学生管理** — 搜索、筛选、查看详情
- **知识点分析** — 全班薄弱环节一目了然
- **暗黑模式** — 护眼主题

## 🚀 使用方法

### 学生练习

1. 克隆仓库
   ```bash
   git clone https://github.com/yizi-wang/TMUA-Practice.git
   ```
2. 用浏览器打开 `index.html` 即可使用，无需安装任何依赖

### 教师看板

1. 用浏览器打开 `dashboard.html`
2. 自动从 QuickForm API 拉取学生成绩数据

## 📁 项目结构

```
├── index.html          # 学生练习界面（含 CSS）
├── dashboard.html      # 教师数据看板 ⭐新增
├── app_local.js        # 应用逻辑
├── questions_data.js   # 题库数据（280 题）
├── images/             # 图形题图片（19 张）
└── .gitignore
```

## 🛠 技术栈

- 原生 HTML / CSS / JavaScript，零依赖构建
- [KaTeX](https://katex.org/) 数学公式渲染
- localStorage 本地持久化存储
- [QuickForm](https://quickform.cn/) 成绩数据收集 ⭐新增

## 🙏 特别感谢

**[QuickForm](https://quickform.cn/)** — 提供简洁高效的数据收集 API，让教师无需搭建服务器即可实时查看学生模考成绩。

- 纯 API 操作，无需打开网页
- 支持 CLI 自动化创建任务
- JSON 格式数据提交，灵活适配各种字段
- 一键导出全部数据

QuickForm 让本项目实现了「学生提交 → 教师看板」的完整闭环，极大提升了教学效率。

## 📝 版本历史

| 版本 | 说明 |
|------|------|
| v1.0 | 280 题题库 + 答题卡侧边栏 + 模拟考试 + 暗黑模式 |
| v2.0 | 成绩提交功能 + 教师数据看板 ⭐新增 |

## ⚖️ 声明

本项目仅供个人学习练习使用，题目版权归 Cambridge Assessment Admissions Testing 所有。
