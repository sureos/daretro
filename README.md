以 Serverless 的方式部署 Trojan

### 快速上手
- 在 Cloudflare Workers 仪表盘中创建一个新的 Worker
- 将 worker.js 文件中的代码粘贴到 Worker 代码编辑器中
- 用你自己的密码替换 `sha224Password`，你可以在 [这里](https://www.atatus.com/tools/sha224-to-hash) 生成密码。或者，你可以之后在 Cloudflare Workers 设置中增加 `SHA224PASS` 环境变量
- 将自定义域名绑定到 Worker
- 访问 `https://[你的域名]/link` 并用你的明文密码替换 `ca110us`

### CF Trojan节点可自定义内容
可修改Trojan_workers_pages文件下的_worker.js文件
1、密码必须自定义（第4行）

2、如果无法访问CF类网站或者ChatGPT，说明ProxyIP失效，可更换ProxyIP，自定义（第5行）

3、伪装网页目前留空，显示为400 Bad Request界面，可自定义（第6行）

也可CF-workers/pages界面中使用变量设置，注：变量设置结果将覆盖本地修改结果
| 变量作用 | 变量名称| 变量值要求| 变量默认值|
| :--- | :--- | :--- | :--- |
| 1、必要的密码 | pswd |任意字符号 |密码：trojan|
| 2、能上CF类网站 | proxyip |ipv4地址、域名、[ipv6地址]|proxyip域名：cdn.xn--b6gac.eu.org|

---------------------------------
### ：查看相关分享链接（单节点，非订阅）
#### CF Trojan分享链接，在网页输入：https:// workers域名 或者 pages域名 或者 自定义域名/自定义密码
