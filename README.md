# EvilOPPOJuice-WCH

OPPO OnePlus ColorOS，BLE广播模拟弹窗，适用于沁恒 CH57X CH58X CH59X 芯片，直接粘贴到沁恒官方例程目录 `/EVT/EXAM/BLE/Broadcaster/APP/broadcaster.c` 文件中，编译烧录即可。

CH57X可能编译报错，`broadcaster.c` 修改此行即可：
```c
extern bStatus_t GAP_UpdateAdvertisingData(uint8_t taskID, uint8_t adType, uint16_t dataLen, uint8_t* pAdvertData);
```
修改为
```c
extern bStatus_t GAP_UpdateAdvertisingData(uint8_t taskID, uint8_t adType, uint8_t dataLen, uint8_t* pAdvertData);
```

* [CH573EVT.ZIP](https://www.wch.cn/downloads/CH573EVT_ZIP.html)
* [CH583EVT.ZIP](https://www.wch.cn/downloads/CH583EVT_ZIP.html)
* [CH592EVT.ZIP](https://www.wch.cn/downloads/CH592EVT_ZIP.html)
