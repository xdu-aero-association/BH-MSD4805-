# BH-MSD4805 Example

## 一、程序简介

- 工程名称：步进电机驱动程序
- 实验平台: 秉火STM32 指南者 开发板 或者 正点原子 精英板 F103ZE
- MDK版本：5.16
- ST固件库版本：3.50

### 功能简介

通过串口发送指令控制步进电机的加减速，按照固定步数移动。按键KEY1和KEY2实现脱机模式与正常工作模式切换。
按键RESET复位操作

### 实验操作

按照以下引脚分配接好线，先接好信号线，电机线，最后才打开电机的电压。通过串口输入指令控制电机的加减速运动，
观察加减速的效果。脱机模式下可以手动旋转步进电机。

### 注意事项

注意设定好步进电机的细分与程序相匹配，电流值要跟所接步进电机相匹配。一般为接近或者小于步进电机的额定电流。

## 二、引脚分配

按键：

|按键编号  |开发板引脚|
|-|-|
|KEY1|PA0 |
|KEY2|PC13|
  
步进电机与开发板相连如下：

|步进电机引脚|开发板引脚  |
|-|-|
|PUL+|PA3 |
|PUL-|GND |
|DIR+|PB14|
|DIR-|GND |
|ENA+|PC4 |
|ENA-|GND |

步进电机:

|步进电机通道|线缆颜色    |
|-|-|
|A+|蓝色线|
|A-|红色线|
|B+|绿色线|
|B-|黑色线|
