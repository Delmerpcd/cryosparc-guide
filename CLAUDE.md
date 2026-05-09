# CryoSPARC 单颗粒冷冻电镜工作流程 · 中文指南

单文件静态网站，位于 `/Users/panchongde/cryosparc-guide/`

- **线上地址**: https://delmerpcd.github.io/cryosparc-guide
- **GitHub 仓库**: git@github.com:Delmerpcd/cryosparc-guide.git
- **访问密码**: `PCD123123123` (staticrypt AES-256 客户端加密)
- **GitHub Pages**: 推送后自动部署，1-2 分钟生效

## 修改流程
1. 编辑 `index.source.html`（源文件，仅存本地，已 gitignore）
2. 加密: `npx staticrypt index.source.html -p PCD123123123 --short`
3. 移动: `mv encrypted/index.source.html index.html`
4. 清理: `rm -rf encrypted .staticrypt.json`
5. 部署: `git add index.html && git commit -m "描述" && git push origin main`

## 网站章节结构（已按学习逻辑排序）
1. 工作流程总览 + 流程图
2. 界面与项目管理（Project/Workspace/Job Builder/Workflows 概念）
3. 第一阶段 · 预处理 — **Import Movies / Patch Motion / Patch CTF / Curate Exposures 含完整参数详解**
4. 第二阶段 · 颗粒挑选（Blob/Template/Topaz Picker → Extract）
5. 第三阶段 · 二维分类（2D Classification → Select 2D）
6. 第四阶段 · Ab-Initio 初始重建
7. 第五阶段 · 精修优化（Homo/Hetero/Non-Uniform Refinement, CTF/Local Refine）
8. 第六阶段 · 后处理验证（Sharpening, Local Resolution, 3DVA, FSC）
9. 快速入门教程 — T20S 蛋白酶体 16 步实战
10. Workflows 自动化详解（创建/应用/Flagged Parameters/导入导出/API）
11. 附录（参数速查表、技巧与常见问题、TRPV1 案例）

## 用户信息
- GitHub: Delmerpcd
- SSH 密钥已配置
- 网站标题: SYSU Urology Lab PCD CryoSPARC 单颗粒分析工作
