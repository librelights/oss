# OSS内网域名与VIP网段对照表

云下机房设备或异地ECS实例希望通过内网访问OSS时，可通过CEN、高速通道、专线、VPN等连接OSS所在地域内网网络，并配置指向OSS内网网段的路由。本文列出OSS各地域的内网网段。

**警告：**

-   OSS为每个Region内网VIP网段划分了固定地址段，您按Region配置路由时必须按照下表地址配置完整的路由，否则可能会造成网络不通。
-   使用ECS实例通过内网访问OSS时，安全组中不能禁止以下任一VIP网段。

|Region|Region ID|VPC网络Endpoint|VIP网段|
|:-----|:--------|-------------|-----|
|华东1（杭州）|oss-cn-hangzhou|oss-cn-hangzhou-internal.aliyuncs.com|-   100.118.28.0/24
-   100.114.102.0/24
-   100.98.170.0/24
-   100.118.31.0/24 |
|华东2（上海）|oss-cn-shanghai|oss-cn-shanghai-internal.aliyuncs.com|-   100.98.35.0/24
-   100.98.110.0/24
-   100.98.169.0/24
-   100.118.102.0/24 |
|华北1（青岛）|oss-cn-qingdao|oss-cn-qingdao-internal.aliyuncs.com|-   100.115.173.0/24
-   100.99.113.0/24
-   100.99.114.0/24
-   100.99.115.0/24 |
|华北2（北京）|oss-cn-beijing|oss-cn-beijing-internal.aliyuncs.com|-   100.118.58.0/24
-   100.118.167.0/24
-   100.118.170.0/24
-   100.118.171.0/24
-   100.118.172.0/24
-   100.118.173.0/24 |
|华北 3（张家口）|oss-cn-zhangjiakou|oss-cn-zhangjiakou-internal.aliyuncs.com|-   100.118.90.0/24
-   100.98.159.0/24
-   100.114.0.0/24
-   100.114.1.0/24 |
|华北5（呼和浩特）|oss-cn-huhehaote|oss-cn-huhehaote-internal.aliyuncs.com|-   100.118.195.0/24
-   100.99.110.0/24
-   100.99.111.0/24
-   100.99.112.0/24 |
|华北6（乌兰察布）|oss-cn-wulanchabu|oss-cn-wulanchabu-internal.aliyuncs.com|-   100.114.11.0/24
-   100.114.12.0/24
-   100.114.100/24
-   100.118.214.0/24 |
|华南1（深圳）|oss-cn-shenzhen|oss-cn-shenzhen-internal.aliyuncs.com|-   100.118.78.0/24
-   100.118.203.0/24
-   100.118.204.0/24
-   100.118.217.0/24 |
|华南2（河源）|oss-cn-heyuan|oss-cn-heyuan-internal.aliyuncs.com|提交工单咨询|
|华南3（广州）|oss-cn-guangzhou|oss-cn-guangzhou-internal.aliyuncs.com|-   100.115.33.0/24
-   100.114.101.0/24 |
|西南1（成都）|oss-cn-chengdu|oss-cn-chengdu-internal.aliyuncs.com|-   100.115.155.0/24
-   100.99.107.0/24
-   100.99.108.0/24
-   100.99.109.0/24 |
|中国（香港）|oss-cn-hongkong|oss-cn-hongkong-internal.aliyuncs.com|-   100.115.61.0/24
-   100.99.103.0/24
-   100.99.104.0/24
-   100.99.106.0/24 |
|美国西部1（硅谷）|oss-us-west-1|oss-us-west-1-internal.aliyuncs.com|提交工单咨询|
|美国东部1（弗吉尼亚）|oss-us-east-1|oss-us-east-1-internal.aliyuncs.com|-   100.115.60.0/24
-   100.99.100.0/24
-   100.99.101.0/24
-   100.99.102.0/24 |
|亚太东南1（新加坡）|oss-ap-southeast-1|oss-ap-southeast-1-internal.aliyuncs.com|-   100.118.219.0/24
-   100.99.213.0/24
-   100.99.116.0/24
-   100.99.117.0/24 |
|亚太东南2（悉尼）|oss-ap-southeast-2|oss-ap-southeast-2-internal.aliyuncs.com|提交工单咨询|
|亚太东南3（吉隆坡）|oss-ap-southeast-3|oss-ap-southeast-3-internal.aliyuncs.com|-   100.118.165.0/24
-   100.99.125.0/24
-   100.99.130.0/24
-   100.99.131.0/24 |
|亚太东南5（雅加达）|oss-ap-southeast-5|oss-ap-southeast-5-internal.aliyuncs.com|提交工单咨询|
|亚太东北1（日本）|oss-ap-northeast-1|oss-ap-northeast-1-internal.aliyuncs.com|提交工单咨询|
|亚太南部1（孟买）|oss-ap-south-1|oss-ap-south-1-internal.aliyuncs.com|-   100.118.211.0/24
-   100.99.122.0/24
-   100.99.123.0/24
-   100.99.124.0/24 |
|欧洲中部1（法兰克福）|oss-eu-central-1|oss-eu-central-1-internal.aliyuncs.com|提交工单咨询|
|英国（伦敦）|oss-eu-west-1|oss-eu-west-1-internal.aliyuncs.com|提交工单咨询|
|中东东部1（迪拜）|oss-me-east-1|oss-me-east-1-internal.aliyuncs.com|提交工单咨询|

