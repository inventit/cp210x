CP210x USB - UART Bridge VCP Driver
===

# 概要

おんどとりとUSBでシリアル通信をするためのLinux用ドライバです。[Silicon Labs](http://www.silabs.com/products/mcu/pages/usbtouartbridgevcpdrivers.aspx)のソースコードに、以下のDevice IDを追加しカスタマイズしています。

```
static struct usb_device_id id_table [] = {
… (snip) …

    { USB_DEVICE(0x0CCF, 0x0500) }, /* TandD USB-UART Controller */

… (snip) …
}
```

# ライセンス

GPL v2

