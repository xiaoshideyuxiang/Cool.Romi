# class B - 系统信息`0x82`

## 0x01.获取系统类型

| 系统      | 值    |
| ------- | ---- |
| iOS     | 0x00 |
| Android | 0x01 |
| Other   | 0xFF |

| 操作 | 接口索引 | 操作数  | 参数   |
| ---- | ---- | ---- | ---- |
| 获取 | 0x82 | 0x01 | xxx |
| 返回 | 0x82 | 0x01 | 系统类型 |

> 例：
> `->APP:^,route,fc,length=2,0x82,0x01,_check_`
> `APP->:^,route,fc,length=3,0x82,0x01,0x00(ios),_check_`
