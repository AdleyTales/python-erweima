# python 代码生成二维码

> 需要的pip包： qrcode

```py

    import qrcode

    qr = qrcode.QRCode(
        version = 7,
        error_correction = qrcode.constants.ERROR_CORRECT_L,
        box_size = 10,
        border = 4
    )

    qr.add_data("http://www.baidu.com/")

    qr.make( fit = True)

    img = qr.make_image()

    img.save("baidu.png")


```
