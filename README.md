# 基于mc生成sram的经典AHB-SRAM设计

### 基于 AHB 的 sram 设计框架图显示如下:

![ahb_sramc_control](https://user-images.githubusercontent.com/71707557/185911793-8c65b49e-e37d-4d1d-b745-6e69bc872b13.png)

### AHB总线传输协议之没有等待状态的单个读写操作:

![没有等待状态的单个传输](https://user-images.githubusercontent.com/71707557/185935469-070d6c22-97d3-4248-958d-b88476e8994c.jpg)

### AHB总线传输协议之有等待状态的单个读写操作:

![插入等待状态的单个读写操作](https://user-images.githubusercontent.com/71707557/185935507-1498f930-3243-45ff-b998-250515906bb2.png)

### AHB总线传输协议之连续读写操作:

![连续读写操作](https://user-images.githubusercontent.com/71707557/185935545-0242f83b-411b-4eb6-9ab1-2d4265828629.png)

### hsize控制读写数据位宽与数据深度(默认位宽为32bit，深度为2^14)

![绘图5](https://user-images.githubusercontent.com/71707557/182754272-dd9540d8-3b8e-4967-a1ff-0342555d659a.png)

### 当hsize为2'b00时，数据位宽为8bit，数据深度为2^16

![fbc7243cd8f6d3286070628d774b1c8](https://user-images.githubusercontent.com/71707557/182756040-11988dca-7215-4767-9a53-8653e4ba6a65.png)

### 当hsize为2'b01时，数据位宽为16bit，数据深度为2^15

![979e27f5082deef4e8b00e63921ec6f](https://user-images.githubusercontent.com/71707557/182756083-7677d5d5-4924-4a9b-aad2-4096af8ff2ab.png)

### 当hsize为2'b10时，数据位宽为32bit，数据深度为2^14

![cdca3ff32af45260c13a686fb47f368](https://user-images.githubusercontent.com/71707557/182756109-daa0d467-e2a6-4313-9f7f-42238b6ffb14.png)

