# CryoSPARC 单颗粒冷冻电镜工作流程 · 中文指南

单文件静态网站，位于 `/Users/panchongde/cryosparc-guide/`

- **线上地址**: https://delmerpcd.github.io/cryosparc-guide
- **GitHub 仓库**: git@github.com:Delmerpcd/cryosparc-guide.git
- **修改后部署**: `git add index.html && git commit -m "描述" && git push origin main`
- **GitHub Pages**: 推送后自动部署，1-2 分钟生效

网站内容基于 CryoSPARC 官方 Guide 整理，涵盖单颗粒冷冻电镜数据处理完整流程：
1. 预处理（Import → Patch Motion → Patch CTF → Curate Exposures）
2. 颗粒挑选（Blob / Template / Topaz Picker → Extract）
3. 二维分类（2D Classification → Select 2D）
4. 三维初始重建（Ab-Initio Reconstruction）
5. 精修优化（Homo/Hetero/Non-Uniform Refinement, CTF Refine, Local Refine）
6. 后处理验证（Sharpening, Local Resolution, 3DVA, FSC）
