# class B - 时间日期`0x01`

## 0x01.获取当前时间日期

| 操作 | 接口索引 | 操作数  | 参数   |
| ---- | ---- | ---- | ---- |
| 获取 | 0x01 | 0x01 | /  |
| 返回 | 0x01 | 0x01 | `年`(0-99),`月`(1-12),`日`(1-31),`时`(0-23),`分`(0-59),`秒`(0-59) |

> 例：
> `->MCU: ^,route,fc,length=2,0x01,0x01,_check_`
> `MCU->: ^,route,fc,length=8,0x01,0x01,year(0-99),month,day,hour,minute,sec,_check_`


## 0x02.设置时间与日期

| 操作 | 接口索引 | 操作数  | 参数   |
| ---- | ---- | ---- | ---- |
| 获取 | 0x01 | 0x01 | `年`(0-99),`月`(1-12),`日`(1-31),`时`(0-23),`分`(0-59),`秒`(0-59) |
| 返回(`ACK`) | 0x01 | 0x02 | / |

> 例：
> `->MCU: ^,route,fc,length=8,0x01,0x02,year(0-99),month,day,hour,minute,sec,_check_`
> `MCU->: ACK`
