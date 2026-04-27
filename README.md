# 📚 TMUA Practice

TMUA（Test of Mathematics for University Admission）在线练习系统，纯前端实现，无需服务器。

## ✨ 功能

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

## 🚀 使用方法

1. 克隆仓库
   ```bash
   git clone https://github.com/yizi-wang/TMUA-Practice.git
   ```
2. 用浏览器打开 `index.html` 即可使用，无需安装任何依赖

## 📁 项目结构

```
├── index.html          # 主页面（含 CSS）
├── app_local.js        # 应用逻辑
├── questions_data.js   # 题库数据（280 题）
├── images/             # 图形题图片（19 张）
└── .gitignore
```

## 🛠 技术栈

- 原生 HTML / CSS / JavaScript，零依赖构建
- [KaTeX](https://katex.org/) 数学公式渲染
- localStorage 本地持久化存储

## 📝 版本历史

| 版本 | 说明 |
|------|------|
| v1.0 | 280 题题库 + 答题卡侧边栏 + 模拟考试 + 暗黑模式 |

## ⚖️ 声明

本项目仅供个人学习练习使用，题目版权归 Cambridge Assessment Admissions Testing 所有。
