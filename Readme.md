#SingleDog

本程序专为双11定制抢单系统，使用方法：
在电脑上（支持Windows，Mac)运行本程序，使用前，使用需要设置好需要抢的商品地址链接，以及用户名和登录密码，系统自动抢京东或者淘宝的打折商品并下单：
为了用户信息保密和安全，本系统不自动支付。
针对淘宝用户，下单成功后，系统自动转支付宝为未支付的订单，用户只需要使用手机刷新支付宝未支付订单进行支付即可；
针对京东用户，下单成功后，系统自动转未支付的订单，用户只需要使用手机刷新手机所有订单状态选择未支付的订单进行支付即可；

反反爬虫策略

禁用 cookie

通过禁用 cookie, 服务器就无法根据 cookie 判断出爬虫是否访问过网站

伪装成搜索引擎

现在可以通过修改 user-agent 伪装成搜索引擎

'Mozilla/5.0 (compatible; Googlebot/2.1; +http://www.google.com/bot.html)',
'Mozilla/5.0 (compatible; Bingbot/2.0; +http://www.bing.com/bingbot.htm)',
'Mozilla/5.0 (compatible; Yahoo! Slurp; http://help.yahoo.com/help/us/ysearch/slurp)',
'DuckDuckBot/1.0; (+http://duckduckgo.com/duckduckbot.html)',
'Mozilla/5.0 (compatible; Baiduspider/2.0; +http://www.baidu.com/search/spider.html)',
'Mozilla/5.0 (compatible; YandexBot/3.0; +http://yandex.com/bots)',
'ia_archiver (+http://www.alexa.com/site/help/webmasters; crawler@alexa.com)',
轮转 user-agent

为了提高突破反爬虫策略的成功率，定义多个user-agent, 然后每次请求都随机选择 user-agent。本爬虫实现了一个 RotateUserAgentMiddleware 类来实现 user-agent 的轮转

代理 IP

使用代理 IP, 防止 IP 被封
