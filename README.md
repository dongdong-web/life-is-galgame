# 人生是一场 Galgame

> 人生不能读档，但你可以记得上一次。

第一版纯静态 MVP。记录「事件 → 选择 → 结局 → 攻略」，数据仅保存在当前浏览器本地。

## 运行

直接打开 `index.html`，或使用任意静态 HTTP Server。

```bash
python -m http.server 8080
```

访问 `http://localhost:8080`。

## GitHub Pages

仓库 Settings → Pages → Deploy from a branch，选择 `main` / root 即可。项目全部使用相对资源路径，可部署在 `用户名.github.io/仓库名/`。

## 当前能力

- 新建、编辑、删除剧情
- 未填写结局自动进入「未完待续」
- 剧情回想、状态筛选、标签筛选、全文搜索
- JSON 导出 / 导入
- 响应式移动端
- 无服务器、无 AI、无钱包、无区块链

## 注意

当前 MVP 使用浏览器 localStorage，而不是最终计划中的 IndexedDB。这样第一版可以做到零构建、直接 GitHub Pages 部署。正式迭代时建议迁移至 IndexedDB/Dexie，并增加客户端加密与链上永久存档。
