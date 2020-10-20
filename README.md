# UART_Tiva_freeRTOS
UART driver example for Tiva Connected TM4C1294XL with FreeRTOS.

This example contains 4 installed tasks, 2 of which compete for UART:
* Terminal
* print_task

Based on the [video series](https://www.youtube.com/watch?v=5JNfTlSQDjI&ab_channel=GustavoDenardin) shared by  [Gustavo Denardin](https://github.com/gustavowd).

## Requirements
* FreeRTOS v10.4.0

The project was developed on **Code Composer Studio Version: 10.1.0.00010**

The CCS Project was created and configurated exactly like the images below:

![img1](./images/project1.png)
![img2](./images/project2.png)
![img3](./images/project3.png)


## How to use
Run the commmand:

```bash
victor@victorUTF:~$ dmesg | grep tty
  [    0.090095] printk: console [tty0] enabled
  [ 1950.239035] cdc_acm 1-1:1.0: ttyACM0: USB ACM device
  [32232.341969] cdc_acm 1-1:1.0: ttyACM0: USB ACM device
```
Connect in **dev/ttyACM0** serial port, using **GtkTerm**, and
set to **115200 8-N-1**.

![img4](./images/project4.png)
