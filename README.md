# Vibe Video 制作流程与技能手册

纯 HTML / CSS / JavaScript 网站，无需 npm 安装或构建。

## 上传 GitHub
1. 解压 ZIP，将 index.html、所有 CSS/JS、README.md 和 .nojekyll 放在仓库根目录。
2. 在 GitHub 创建名为 vibe-video 的仓库。
3. 点击 Add file → Upload files，上传解压后的文件（不是 ZIP 本身），提交更改。

## 使用 GitHub Pages 发布
1. 免费账户可使用公开仓库发布。
2. Settings → Pages → Build and deployment。
3. Source 选择 Deploy from a branch。
4. Branch 选择 main，目录选择 / (root)，保存。
5. 等待部署完成，访问 https://你的用户名.github.io/vibe-video/ 。
注意：GitHub Pages 网站默认公开访问，与原 Sites 网站的私有权限不同。

## 本地预览
在文件所在目录运行：
python -m http.server 8000
然后打开 http://localhost:8000 。

## 文件说明
- index.html：页面结构
- app.js：六阶段导航与 GitHub 同步
- library.js：制作手册与方法内容
- motion.js：首页流程动效
- style.css / refined.css / library.css / motion.css：对应样式

## 后续更新
修改并提交文件后，GitHub Pages 自动重新发布。
GitHub 指标在网页打开时检查，使用浏览器缓存；请求受 GitHub 匿名 API 限流约束。
中文教程为手工编辑，不会因仓库更新自动改写。
Google Fonts 与 GitHub API 需要网络连接。
本导出包包含当前网站源码，不含 Git 历史、Sites 身份配置或任何 API 密钥。
以后在 Sites 中修改原站，不会自动同步到你的 GitHub 仓库，反之亦然。
教程中引用的第三方项目仍遵循各自许可证；教程所列的 skills 和模型不包含在本包内。
