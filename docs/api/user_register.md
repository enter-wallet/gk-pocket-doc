# 新用户注册
URL: `/external/register`  
Method: `POST`

> 参数   

| 参数名        | 类型         | 是否必须   | 描述                                | 例子                 |
| ------------ | ----------- | --------- | ---------------------------------- | -------------------- |
| netSource    | string      | YES       | 用户来源                            |  A01/A02/A03 等      |
| phone        | string      | YES       | 用户手机号，用Base64编码              | MTMONTU2Nj=          |
| countryCode  | string      | YES       | 手机号国际区号                       | 86/63/886 等          |
