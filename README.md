BluetoothProgramming
====================
這是一份使用 C/C++ 語言寫 Bluetooth 通訊的教學  
資料來源是參考下列的原文資料  
[An Introduction to Bluetooth Programming](https://people.csail.mit.edu/albert/bluez-intro/index.html)  
適合於入門藍芽開發者、寫過 socket 程式的更容易上手.  


## 安裝開發套件
Ubuntu 使用下列指令安裝開發套件函式庫  
```
sudo apt-get install libbluetooth-dev libbluetooth3
(sudo apt-get install python-bluez)
```

## 如何編譯與使用
執行下列指令進行編譯  
```
mkdir build
cd build
cmake ..
make
```
進入下列目錄執行編譯好的執行檔  
```
cd bin
./simplescan
```
## 藍芽基本指令
查看藍芽裝置  
```
hciconfig
```

掃描附近的藍芽裝置  
```
hcitool scan
```

make your device discover-able  
```
sudo hciconfig hci0 piscan
sudo hciconfig hci0 name 'Device Name'
```

## 程式介紹
* SimpleScan
    簡單的掃描.
* RFCOMM
    使用 RFCOMM Sockets 來做簡單的 server/ client 通訊.
* L2CAP
    使用 L2CAP Sockets 來做簡單的 server/ client 通訊.

## Reference
[Chapter 4. Bluetooth programming in C with BlueZ](https://people.csail.mit.edu/albert/bluez-intro/c404.html)  
[4.2. RFCOMM sockets](https://people.csail.mit.edu/albert/bluez-intro/x502.html)  
[4.3. L2CAP sockets](https://people.csail.mit.edu/albert/bluez-intro/x559.html)  
[用Raspberry 來玩 blue tooth programming PyBluez](http://0975128810.blogspot.tw/2016/01/raspberry-blue-tooth-programming-pybluez.html)  
