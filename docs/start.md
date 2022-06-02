# 准备
### 1.接口调用准备
> 接口请求方法：POST  
>
> 接口参数类型：JSON  
>
> 接口签名算法：SHA256withRSA  
>
> 接口Header必填参数，如下：  

| name         | value       | description               |
| ------------ | ----------- | ------------------------- |
| Content-Type | application | 指定请求参数格式JSON         |
| appid        |             | 各网站的商户代码，由交易所分配 |
| sign         |             | 参数签名                   |