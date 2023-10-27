# samltooltest
TEST ระบบ saml 
# ขั้นตอนการติดตั้ง
- Clone ตัว REPO
- ตั้้งค่า Loopback mapping ไปที่ "sp.samltools.com". (ตัวอย่างการรันนี้ รันผ่าน Terminal บน mac)

```
ตั้งค่า host เข้า ใช้คำสั่ง sudo nano /etc/hosts และเพิ่ม 127.0.0.7 sp.samltools.com
รัน sudo ifconfig lo0 alias 127.0.0.7 up
```

- เปิดตัว Service provider

```
$ cd sp
$ go run samlsp.go
```

- เท่านี้ก็เข้าไปที่เว็บ "http://sp.samltools.com:4567/pages/sp.html" ใน Browser

