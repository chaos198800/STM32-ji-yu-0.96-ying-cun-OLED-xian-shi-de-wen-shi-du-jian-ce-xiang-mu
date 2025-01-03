# STM32基于0.96英寸OLED显示的温湿度监测项目

本仓库提供了一个利用STM32单片机，结合0.96英寸OLED显示屏和DHT11温湿度传感器进行温湿度测量与显示的完整示例项目。项目实现了温湿度数据的实时获取、在OLED屏上显示以及通过串口监控温度和湿度值的功能。非常适合初学者学习STM32、OLED显示技术以及DHT11传感器的应用。

## 技术规格

- **MCU**: STM32F10x系列
- **显示模块**: 0.96英寸OLED显示屏
- **环境传感器**: DHT11温湿度传感器
- **通信接口**: UART（用于串口打印）
- **系统时钟**: 配置为72MHz

## 文件包含

- `stm32f10x.h`：STM32的基础库文件。
- `OLED.h`：OLED显示屏驱动头文件。
- `led.h`：LED控制相关的函数定义。
- `usart1.h`：串口1的配置和操作函数。
- `delay.h`：延时函数实现。
- `dht11.h`：DHT11温湿度传感器驱动程序。

## 主要功能

1. **初始化**：包括STM32的系统初始化，OLED显示屏初始化，LED和串口的配置。
2. **温湿度采集**：通过DHT11传感器读取当前的温度和湿度值。
3. **数据显示**：将获得的温湿度信息在0.96英寸OLED屏幕上显示。
4. **串口打印**：通过串口发送当前的温湿度数据，便于在电脑端监控。

## 使用说明

1. **编译与烧录**：确保您已安装好STM32的相关开发环境如Keil MDK或STM32CubeIDE，然后打开项目工程，编译并通过ST-LINK等工具烧录到STM32芯片中。
   
2. **连接传感器**：正确连接DHT11至STM32，通常使用单个GPIO引脚加上拉电阻的方式连接。
   
3. **OLED显示屏接线**：遵循OLED显示屏的接线指导，一般涉及SPI/I2C通信接口。

4. **串口监听**：使用串口助手软件（如RealTerm或SecureCRT），设置适当的波特率（如9600）来接收并查看串口输出的数据。

5. **调试与优化**：根据实际显示效果调整代码中的延时参数或显示逻辑，确保数据准确无误地显示与传输。

## 注意事项

- 确保所有外设的电压和通信协议与STM32兼容。
- 在编写或修改代码前，请详细阅读相关硬件的数据手册以避免错误配置。
- 调试过程中，观察串口输出可以帮助快速定位问题。

加入我们，一起探索嵌入式世界的奥秘，通过这个项目，你不仅能够掌握STM32的基本应用，还能深入了解如何结合外部传感器和显示设备进行综合设计。祝你学习愉快！

## 下载链接

[STM32基于0.96英寸OLED显示的温湿度监测项目](https://pan.quark.cn/s/ad430d3f1077)