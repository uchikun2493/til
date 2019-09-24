# Arduinoの設定

## ubuntu

USBで接続されているポート名の確認

```
$ ls -l /dev/serial/by-id/
```
自分の手元では以下のような出力になった
usb-FTDI_FT232R_USB_UART_A906ORL3-if00-port0 -> ../../ttyUSB0

書き込み権限の確認

```
$ ls -la /dev/ttyUSB0 
```

出力例
crw-rw---- ...

書き込み権限がなければ変更する

```
$ sudo chmod 666 /dev/ttyUSB0 
$ ls -la /dev/ttyUSB0 
```

出力例
crw-rw-rw- ...


