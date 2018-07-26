# aliwxpay
把支付宝微信的收款码合并一个二维码

把支付宝微信的收款码合并一个二维码，无论用微信还是支付宝扫这个码均可支付
思路： 微信，支付宝收款码均是一堆字符型。只要我们的二维码是对应的串， 微信 支付宝就能识别。
合并的二维码包含里面同时包含支付宝微信的收款码。如果是微信扫码，识别出是来自微信扫码，生成微信的收款码即可。
由于支付宝的收款码本身是一个链接，可以打开，所以判断是来自支付宝扫码，直接跳转至支付宝的收款码链接即可。

使用步骤 
1 启动一个服务器
2 获取本项目在服务器的地址，然后传参数，实际开发中 收款码建议加密，js去解密
http://192.168.1.130:3000/?ali=HTTPS://QR.ALIPAY.COM/FKX041987IXG0B6BVSBRE2?t=1532515010748&wx=wxp://f2f0HFQwzbh4N2vtBV-KO-v9HDXOKWeGz64e

ali=HTTPS://QR.ALIPAY.COM/FKX041987IXG0B6BVSBRE2?t=1532515010748&wx=wxp://f2f0HFQwzbh4N2vtBV-KO-v9HDXOKWeGz64e （分别是支付宝与微信的收款码）


将http://192.168.1.130:3000/?ali=HTTPS://QR.ALIPAY.COM/FKX041987IXG0B6BVSBRE2?t=1532515010748&wx=wxp://f2f0HFQwzbh4N2vtBV-KO-v9HDXOKWeGz64e
这个链接用二维码工具生成一个二维码，然后微信 或者支付宝扫码即可。

完毕
