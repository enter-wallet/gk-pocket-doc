# 获取链接及二维码（用于交易所扫码或跳转上分）
URL: `/external/encrypt`  
Method: `POST`

> 参数   

| 参数名        | 类型         | 是否必须   | 描述                                | 例子                 |
| ------------ | ----------- | --------- | ---------------------------------- | -------------------- |
| loginName    | string      | YES       | 用户交易所账号                       |  10                  |
| amount       | number      | YES       | 上分金额，必须大于0                   |  10                  |
| currency     | string      | YES       | 币种                                | USDT/USDC/ETH等      |
| protocol     | string      | NO       | 协议，currency为USDT/USDC时必传       | ERC20/TRC20/BEP20/POLYGON |
| address      | string      | YES       | 数字币地址                          | ERC20/TRC20/BEP20/POLYGON |

> Request   

```json
{
    "loginName": "DK10660",
    "address": "0xb53615767Ee61E1628bCD87Ff95d8112c4e18Bb4",
    "currency": "USDT",
    "protocol": "ERC20",
    "amount": "10"
}
```

> Response   

```json
{
    "head": {
        "code": "0000",
        "message": "成功",
        "fieldErrs": null
    },
    "body": {
        "qrcode": "x70KtodkgieurJIUHKJNFjjdhdghdjfdjfjdhjfndsjfbhdbfhgdhfhsbUHUIU4t9x70KtodkgieurJIUHKJNFjjdhdghdjfdjfjdhjfndsjfbhdbfhgdhfhsbUHUIU4t9x70KtodkgieurJIUHKJNFjjdhdghdjfdjfjdhjfndsjfbhdbfhgdhfhsbUHUIU4t9",
        "appUrl": "gkpocket://pay?text=x70KtodkgieurJIUHKJNFjjdhdghdjfdjfjdhjfndsjfbhdbfhgdhfhsbUHUIU4t9x70KtodkgieurJIUHKJNFjjdhdghdjfdjfjdhjfndsjfbhdbfhgdhfhsbUHUIU4t9x70KtodkgieurJIUHKJNFjjdhdghdjfdjfjdhjfndsjfbhdbfhgdhfhsbUHUIU4t9",
        "webUrl": "https://gkpmob-w.uatdesk.com?text=x70KtodkgieurJIUHKJNFjjdhdghdjfdjfjdhjfndsjfbhdbfhgdhfhsbUHUIU4t9x70KtodkgieurJIUHKJNFjjdhdghdjfdjfjdhjfndsjfbhdbfhgdhfhsbUHUIU4t9x70KtodkgieurJIUHKJNFjjdhdghdjfdjfjdhjfndsjfbhdbfhgdhfhsbUHUIU4t9"
    }
}
```