## 开通网关权限
目前 API 网关在内测阶段，您需要在 https://cloud.tencent.com/product/apigateway 中点击申请内测开通 API 网关，或联系自己的客户经理直接申请开通。开通后，您就可以进入 API 网关的管理控制台进行配置了。

## 服务创建
1. 登陆 [腾讯云管理控制台](https://cloud.tencent.com/login?s_url=https%3A%2F%2Fcloud.tencent.com%2F)，选择 API 网关产品
![控制台产品列表](https://i.imgur.com/kE0GJKa.png)

2. 在当前地域下，服务标签页中，单击【新建】
![新建服务](https://i.imgur.com/DsnOFaH.png)

3. 填写服务名称、备注信息，并选择前端类型，前端类型可选择 http、https、http 与 https 任一种
![服务信息](https://i.imgur.com/lG0WNAh.png)
> 服务名有特定输入限制，包括：不区分大小写，均以小写体现，可包含数字，不可包含其他非数字和字母外的符号，长度限制为 30 字符。

4. 单击【完成】，服务创建成功，可进入 API 管理进行 API 创建
![服务创建成功](https://i.imgur.com/pLKCOm4.png)


## API创建
1. 进入服务的 API 管理标签页中，单击【新建】
![API管理](https://i.imgur.com/MRJOlEd.png)

2. 进行前端配置和后端配置

## 前端配置
配置说明：
1）配置您需要访问的路径，如：/path

2）选择您需要的请求方法，目前有：GET、POST、PUT、DELETE、HEAD

3）选择性的输入备注信息

4）根据提示填写你的 API 需要的入参配置

5）单击【下一步】进入后端配置
![前端配置](https://i.imgur.com/ieIGQVj.png)

**注意：如果您是 API 市场的供应商，在部署即将售卖的 API 时，请勿选择免鉴权。**

## 后端配置
一般 API 市场的供应商，后端配置均为 http 对接，故此处仅讲解 http 配置。如需了解其他后端配置，请参考 API 网关文档

配置说明：
1）后端对接 http 时，需要选择您的后端类型为 http 或 https

2）输入后端地址，以 http:// 或 https:// 开头，不包括后面的路径，例如 "http://api.myservice.com" 或 "http://108.160.162.30"

3）输入后端路径以/开头，如 /path 或 /path{petid}

4）选择请求方法，前后端选择的请求方法可不一致

5）设置后端超时时间

6）设置映射前端的后端参数

7）单击【完成】
![后端配置](https://i.imgur.com/pQfgDqp.png)

## API调试
当 API 创建完成后，您可对 API 进行调试

1. 进入 API 管理页面，选择需要调试的 API，单击右上角的【 API 调试】按钮进入调试页面
![API调试](https://i.imgur.com/G6nTTsP.png)

2. 输入调用 API 的默认参数，单击【发送请求】
![API调试](https://i.imgur.com/quIudJS.png)

3. 右侧会展示调用 API 的返回结果
![API调试返回结果](https://i.imgur.com/JRSy6my.png)

##服务发布
您创建的服务以及服务中的 API，需要发布，才能进行访问

1. 进入服务列表，选择需要发布的服务，单击其右边的【发布】按钮
![发布](https://i.imgur.com/u2b5FBa.png)

2. 选择需要发布服务的环境，目前支持测试，预发布，发布三种环境；单击【完成】，即可进行调用
![选择发布环境](https://i.imgur.com/HO62H0y.png)

**注意：作为 API 市场可发布的产品，您需要将您要发布的 API 服务发布到发布环境中**

服务发布后，您可以自行调用，也可以进入 API 市场创建要售卖的 API。
若您需要自行调用。需要创建响应的密钥与使用计划，具体创建请参考：https://cloud.tencent.com/document/product/628  中的使用计划与密钥


