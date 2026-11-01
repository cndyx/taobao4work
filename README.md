# Taobao4Work

面向工作采购的独立 Codex Skill，使用 Playwright CLI 查询本人淘宝/天猫订单。

## 当前状态

订单查询、金额口径、退款与物流核对流程已定义；尚未完成真实淘宝账号的端到端验证。本项目是代理操作说明，不是淘宝 API SDK 或无人值守爬虫。

## 安装

使用 Codex 内置 skill-installer 安装本仓库根目录，安装名为 taobao4work；同时安装 openai/skills 的 skills/.curated/playwright。需要 Bash、Node.js/npm，并在可见浏览器里手动登录。

示例：`使用 $taobao4work 查询我最近的淘宝订单。`

## 后续计划（尚未实现）

- 按 BOM 匹配商品及 SKU，按授权加购。
- 自助开票与人工客服索票。
- 本地 Excel 账簿交互、发票原件关联及贴入。

详见 [扩展规范](references/extensions.md)。

## 数据与操作

仓库不包含订单、凭证或浏览器登录态。默认只读查询；不付款、不确认收货、不修改订单。工具权限与网站验证仍适用，Playwright 不用于规避安全拒绝。
