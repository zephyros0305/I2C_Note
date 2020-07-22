# I2C Note

* **Two open drain line**
    * SCL - Serial Clock Line, holds Clock signal
    * SDA - Serial Data Line, holds Data or address signal

* **One to many**
    * one master with one or more slaves.

* **Speed**
    * Standard mode - 100kHz (100kbits/s)
    * Fast mode - 400kHz (400kbits/s)
    * Fast mode plus - 1MHz (1Mbits/s)
    * High speed mode - 3.4MHz (3.4Mbits/s)
    * Ultra fast mode - 5MHz (5Mbits/s) **\*only master to slave**

* **SCL**
    * SCL為Low時, SDA可以改變資料.
    * SCL為High時, SDA必需保持訊號穩定, 不可以改變.
    * 特殊情況下SCL為High時, SDA可改變(Start & Stop).

* **SDA**
    * Start bit - Falling edge
    * Stop bit - Raising edge
    * ACK - SDA drive low
    * NACK - SDA pull up

* **Data composed**
    ![](https://i.imgur.com/ZXUbhtE.png)
    


---
### Ref
https://magicjackting.pixnet.net/blog/post/173061691-i2c-bus-%E7%B0%A1%E4%BB%8B-(inter-integrated-circuit-bus)
https://www.coderbridge.com/@bcewang/ecce611429114a0687b74f014da0659a
http://wiki.csie.ncku.edu.tw/embedded/I2C#ic-speed