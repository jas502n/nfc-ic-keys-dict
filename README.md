# nfc-ic-keys-dict
 2021-05-31 nfcPro.exe 早期版本下载 

http://www.nsccn.com/web/soft/win/20210531/nfcPro.exe

![image](https://user-images.githubusercontent.com/16593068/171908353-736768cc-4e3c-465b-8d54-921a3175baf4.png)

keys for ic: `1D14130D1A0B/000000000000`

## 如何检测iC卡`类型`：

`谷歌商店 =>> MIFARE Classic Tool =>> 工具 =>> 显示标签信息`

```
UID: xxxxx (4 byte)
RF 技术：ISO/IEC 14443, Type A
ATQA: 0004
SAK: 08
ATS: - 
标签类型和制造商：MIFARE Classic 1k, NXP
内存大小：1024 byte
块大小：16 byte
扇区数：16
块数：64
```
![image](https://user-images.githubusercontent.com/16593068/171908148-b28c3a76-410b-48a2-a76d-25d121b38521.png)


NFC数据分析：

![image](https://user-images.githubusercontent.com/16593068/171986488-a067734e-0396-4c62-acdf-4acd42413de4.png)

接口1：
`http://50216831.cn-shanghai.fc.aliyuncs.com/2016-08-15/proxy/NFCReaderTools/liftanalyze/?data=<hex_data>`

接口2：
`http://50216831.cn-shanghai.fc.aliyuncs.com/2021-04-06/proxy/NFCReaderTools/liftanalyze/?data=<hex_data>`

![image](https://user-images.githubusercontent.com/16593068/171986435-8258a256-3a32-44be-bf21-68752de49d36.png)

### 加密卡
```bash

检测到以下信息：
鼎博门禁 - 2066.1.1 - 所在扇区:2
无名门禁15 - 2021.10.14 - 所在扇区:6
此分析由夏天IC助手提供,分析结果仅供参考，详情访问http://ic.aec8.com:88/zx.php
```

### 空白卡

```
检测到以下信息：
空白卡 - 所在扇区:0
这是一张空白卡！
此分析由夏天IC助手提供,分析结果仅供参考，详情访问http://ic.aec8.com:88/zx.php
```

## 2次数据对比

`两个文件总计有67个字节不同，分布在9个块内`
![image](https://user-images.githubusercontent.com/16593068/171986679-609f9dc1-1dce-4ca0-9609-f4469cddfe99.png)

