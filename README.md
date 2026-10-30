# pure-math-taxonomy

中小学·高中知识图谱（纯净版）——数学、语文、英语、物理四科知识点 DAG，附自适应前置诊断与题库。

基于 [xiaoyang111222/cn-math-taxonomy](https://github.com/xiaoyang111222/cn-math-taxonomy)（MIT）重构，感谢原作者的工作。

## 本版本做了什么

- 移除站内所有第三方推广内容（智商测试入口、资源搜索等）
- 断开第三方统计上报，分享二维码/水印不再指向外部站点
- 纯静态部署：任何静态服务器/Nginx/CDN 直接托管，零构建

## 功能

- 对齐《义务教育数学课程标准（2022 年版 2025 年修订）》《普通高中数学课程标准（2017 年版 2025 年修订）》必修+选择性必修，人教版教材
- 知识图谱可视化（小学/初中/高中分色，硬先修实线、软先修虚线）
- 自适应诊断：答错沿先修边回溯薄弱根因，给出按年级排列的学习路径
- 孩子档案：本地 localStorage 保存多个孩子的诊断历史与薄弱点，数据不出本机
- PWA 离线可用

## 使用

纯静态站点，克隆后任意 HTTP 服务器托管根目录即可：

```bash
git clone https://github.com/sijie-yin/pure-math-taxonomy.git
cd pure-math-taxonomy
npx serve .
```

## 目录结构

- `index.html` 首页（按年级进入）
- `explore/` 知识图谱浏览
- `diagnose/` 自适应诊断工具
- `children/` 孩子档案与历史记录
- `data/` 知识点 DAG 与题库（JSON）
- `assets/` 样式与脚本

## 许可

继承原项目 MIT License。

---
*AI 参与重构（内容清理与部署），基于开源项目 cn-math-taxonomy。*
