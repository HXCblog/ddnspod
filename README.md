# DNSPod IP 刷新脚本

自动获取域名ID与记录ID。
只需要修改config即可运行，没有做错误处理建议安装supervisor，并由supervisor启动。

所需修改如下所示：
```python
config = {
    "ID": 10000,                                # 填写你自己的API Token ID
    "TokenID": "xxxxxxxxxxxxxxxxxxxxxxxx",      # 填写你自己的API Token
    "domains":{
        "youdomain.info": ['www', 'ftp']        # 填写需要更新的域名及对应的记录
    },
    "delay": 10                                 # 检查时间
}
```

