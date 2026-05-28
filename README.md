# BLOG_TITLE

基于 Hexo 和 Hexo Theme Fluid 的个人技术博客模板。

## 本地开发

```bash
npm install
npm run server
```

本地预览地址：

```text
http://localhost:4000/
```

## 常用命令

```bash
npm run clean
npm run build
npm run server
npm run deploy
```

- `clean`：清理 Hexo 缓存和生成目录。
- `build`：生成静态文件到 `public/`。
- `server`：启动本地预览服务。
- `deploy`：清理后重新生成静态文件，适合上线前检查。

## 个性化占位符

发布前建议搜索并替换这些占位符：

- `BLOG_TITLE`
- `BLOG_SUBTITLE`
- `BLOG_DESCRIPTION`
- `BLOG_DOMAIN`
- `BLOG_KEYWORDS`
- `AUTHOR_NAME`
- `AVATAR_URL`
- `GITHUB_URL`
- `EMAIL_ADDRESS`
- `TECH_STACK`
- `PROJECT_DIRECTION`
- `WRITING_TOPICS`

主要配置文件：

- `_config.yml`：Hexo 站点配置。
- `_config.fluid.yml`：Fluid 主题配置。
- `source/_posts/`：博客文章。
- `source/about/index.md`：关于页。
- `vercel.json`：Vercel 构建配置。

## 部署到 Vercel

1. 新建 GitHub 或 GitLab 仓库。
2. 将当前目录推送到远程仓库：

   ```bash
   git remote add origin YOUR_REPOSITORY_URL
   git branch -M main
   git push -u origin main
   ```

3. 在 Vercel 中导入该仓库。
4. 使用以下构建配置：

   ```text
   Framework Preset: Other
   Install Command: npm install
   Build Command: npm run build
   Output Directory: public
   Node.js Version: 20.x or newer
   ```

5. 部署完成后，把 `_config.yml` 中的 `url` 从 `https://BLOG_DOMAIN` 改为真实域名或 Vercel 分配的地址。
