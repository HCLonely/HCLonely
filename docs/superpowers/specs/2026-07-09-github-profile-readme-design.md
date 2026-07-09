# GitHub 个人主页 README 改版设计

## 目标

将现有仅包含访问量、社交链接和统计卡片的 README，改造成兼顾个人辨识度与项目展示的平衡型个人主页。页面应突出 HCLonely 的开源项目、前端与自动化技术方向，同时保持简洁、稳定且适合 GitHub 原生 Markdown 渲染。

## 视觉方向

- 采用深色蓝青色调，通过 GitHub 兼容的图片、徽章和 HTML 对齐属性形成视觉层级。
- 不引入复杂动画、脚本或无法在 GitHub README 中运行的自定义样式。
- 控制页面长度和信息密度，保证桌面端与移动端均可顺畅阅读。
- 使用清晰的小节、项目卡片和统计卡片，避免装饰元素压过核心内容。

## 内容结构

1. 顶部欢迎区
   - 主标题：`Hi, I'm HCLonely 👋`
   - 个人表达：`艺术家思维去思考问题，工匠创造精神去开发`
   - 访问量徽章
2. 个人简介
   - 简要说明关注方向：开源工具、Hexo 生态、Web 开发与自动化。
3. 精选项目
   - `hexo-bilibili-bangumi`
   - `hexo-theme-webstack`
   - `all-pusher-api`
   - `Artitalk`
   - 每个项目展示名称、用途和主要技术，不写死容易过期的 Star 数。
4. 技术栈
   - JavaScript
   - TypeScript
   - HTML
   - CSS
   - Node.js
   - Git
5. 外部链接
   - Blog
   - GitHub
   - 不展示 Twitter。
6. 数据展示
   - GitHub Stats
   - Top Languages
   - WakaTime

## 外部服务与降级

- 统计卡片继续使用公开图片服务，不在 README 中加入运行时代码。
- 所有图片提供有意义的 `alt` 文本；外部图片加载失败时，核心简介和项目链接仍然可用。
- 项目与社交链接使用明确的 HTTPS 地址。
- 避免依赖动态 Star 徽章，以减少视觉噪声和第三方请求。

## 验收标准

- README 在 GitHub Markdown 中无明显排版错误。
- 四个精选项目均链接到 HCLonely 名下对应仓库。
- 页面仅包含 Blog 与 GitHub 两个外部身份入口，不包含 Twitter。
- 技术栈、项目简介和个人定位与公开仓库内容一致。
- 不包含占位文本、失效的相对资源或自定义 JavaScript。
- 保留 GitHub Stats、Top Languages、WakaTime 和访问量信息。
