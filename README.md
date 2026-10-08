# 正在忙.exe · V1.1

中文摸鱼互动网站，基于 React 19 + Vite 6。

## 功能

- 首页与移动端响应式布局
- Ctrl/⌘ + Shift + X 一键打开或关闭虚构办公报表，Esc 退出
- 5题职场人格测试与分享
- 带薪钓鱼（抛竿、随机咬钩、收杆、鱼获收藏）
- 基于浏览器 localStorage 的本机访问、游戏和停留统计

注意：本版本没有远端数据库、全站访问分析、登录、支付、企业营销后台。

## 本地运行

```bash
npm install
npm run dev
```

## 构建

```bash
npm run build
```

输出在 `dist/`。GitHub Actions 会在推送时进行云端编译检查。

## Cloudflare Pages

1. 在 Cloudflare 控制台 Workers & Pages 创建 Pages 项目，并连接本 GitHub 仓库 `zhihanglin997-prog/-`
2. Production branch: `main`
3. Framework preset: `Vite`
4. Build command: `npm run build`
5. Build output directory: `dist`
6. Root directory: `/`
7. 点击 Save and Deploy。成功后 Cloudflare 会提供 `*.pages.dev` 地址。

**部署成功前不要把 GitHub 仓库地址当作网站网址。**
