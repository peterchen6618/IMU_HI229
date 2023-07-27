# IMU_HI229
## Synopsis 概要
本專案為讀取超核公司HI229的IMU資料，解碼並且打印至終端上，本專案之API函數可以選擇要打印的資料包。

## Getting Started 使用指南

### Prerequisites 項目使用條件

- 測試環境：Windows10_x64 作業系統

- 編譯器：keil_V5.37.0

- 開發板：STM32F407G-DISC1
	
- 測試設備：超核科技HI229

### Installation 安装
本專案使用HAL庫開發，STM32與HI229連接腳位如下:

| STM32 | HI229 Pin |
| ----- | --------- |
| PA2   | RXD       |
| PA3   | TXD       |

### Usage example 使用示例
本專案撰寫了HI229的API函數如下:

```C
// 打印IMU資料
void dump_data_packet(receive_imusol_packet_t *data);
```
## Reference 參考
- [HI229-Git][1]

  [1]: https://github.com/peterchen6618/IMU_HI229  "游標顯示"
