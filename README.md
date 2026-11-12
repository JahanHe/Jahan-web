# 个人网站预发布环境

当前只部署“等待上传 Demo”的占位页，没有上传个人网站内容或私人资料。

预发布地址：https://jahanhe.github.io/mr-he-preview/

## 部署方式

使用 GitHub Pages 原生分支发布：`main` 分支的 `/docs` 目录。每次推送该目录的变更，GitHub 自动构建和发布，无需另买服务器或单独保存部署密钥。

仓库和预发布网页都是公开的。占位页设置 `noindex`，请求搜索引擎不收录；这不是密码保护。

## 收到 Demo 后

1. 确认交付的是 HTML 静态文件、需要构建的前端项目，还是依赖服务器的应用。
2. 只将审核后的公开网页产物放入 `docs/`，不要把整个工作目录、备份、私密资料或密钥提交到仓库。
3. 检查资源路径适配 `/mr-he-preview/` 子目录；首页须为 `index.html`。需要后端的功能另行确定服务，GitHub Pages 本身只托管静态文件。
4. 提交并推送，检查 Pages 构建结果，再核验在线首页和关键资源。更新有问题时用 Git revert 回退相应提交并重新发布。

## 域名与后续国内版本

当前可直接使用 GitHub 的 HTTPS 地址。选好并购买自有域名后，可验证域名所有权、配置 DNS，再绑定 Pages；无需现在购买服务器。

阿里云国内正式版单独规划服务器、备案和发布。此预发布环境不替代国内访问体验测试，也不提供私有后台或数据库。

参考：[GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages)、[配置分支发布](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)。
