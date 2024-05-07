以 Serverless 的方式部署 Trojan

### 快速上手
- 在 Cloudflare Workers 仪表盘中创建一个新的 Worker
- 将 worker.js 文件中的代码粘贴到 Worker 代码编辑器中
- 用你自己的密码替换 `sha224Password`，你可以在 [这里](https://www.atatus.com/tools/sha224-to-hash) 生成密码。或者，你可以之后在 Cloudflare Workers 设置中增加 `SHA224PASS` 环境变量
- 将自定义域名绑定到 Worker
- 访问 `https://[你的域名]/link` 并用你的明文密码替换 `ca110us`
