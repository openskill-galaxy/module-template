# OpenSkill Galaxy 学习模块模板

课程、讲义、题库、考试和案例共用同一套静态站点模板。[查看在线模板](https://openskill-galaxy.github.io/module-template/)

| 学习环节 | 提供的功能 |
| --- | --- |
| 阅读和续学 | 课程、讲义、学习路线、章节目录、收藏与笔记 |
| 练习和复习 | 按章或按状态筛选、到期复习、模拟考试和错题本 |
| 作答和收回反馈 | 案例草稿、Markdown 导出、送审和评语导回 |
| 管理学习数据 | 浏览器本地保存、备份恢复、可选 Appwrite 同步 |

## 本地开发

使用 Node.js 22。数据位于 `public/data/`，共享界面位于 `src/`。

```bash
npm ci
npm run dev
node scripts/validate-data.mjs
npm run build
npm run preview
```

## 新建和维护模块

复制模板后，为新模块设置 `module.json`、包名、Vite 部署路径、网页元数据和 PWA 作用域。填入实际课程数据，生成搜索索引并校验。主站纳入新模块后，刷新目录、统计和全局索引。维护共享界面时，从此模板运行传播检查，核对需要同步的文件。

[完整模块工作流](https://github.com/openskill-galaxy/openskill-galaxy-tools/blob/main/MODULE_WORKFLOW.md) · [GitHub Pages 发布核验](https://github.com/openskill-galaxy/openskill-galaxy-tools/blob/main/GITHUB_PAGES_DEPLOY_GUIDE.md) · [MIT 许可](https://opensource.org/license/mit)
