# 极简 GitHub Pages（Markdown 驱动）

## 结构
```
/
├─ index.html
└─ posts/
   ├─ posts.json
   ├─ hello-world.md
   └─ second.md
```

## 部署
- 新建仓库并开启 **Settings → Pages → Deploy from a branch**（`main` / root）。
- 把以上文件原样上传到仓库根目录。
- 打开 `https://<你的用户名>.github.io`（或 `/<仓库名>/`）。

## 写新文章
1. 在 `posts/` 里新增 `你的slug.md`。
2. 在 `posts/posts.json` 里添加：
```json
{ "slug": "你的slug", "title": "文章标题", "date": "YYYY-MM-DD" }
```
3. 在网页的「博客」里就会出现了，点击即可阅读。

> 备注：纯静态站点无法列目录，所以使用一个小小的 `posts.json` 清单来帮助前端生成列表。
