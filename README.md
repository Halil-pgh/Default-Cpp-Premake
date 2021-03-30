# Default C++ Premake

## Projeyi çalıştırma

### Linux için çalıştırma

Bu proje, kurmak için **make**, debugging için **gdb** kullanıyor.
Eğer bu programlar yoksa indirmeniz lazım.
>Arch'da
```
sudo pacman -S base-devel
```
>Ubuntu'da
```
sudo apt install build-essential
```

İhtiyacınız olan aletleri aldığınıza göre şimdi ana projeyi vscode'da
açın. Ctrl + Shift + B yaparsanız premake'i çalıştıracaktır. Sonucunda
bir tane projenin altında, bir tane workspace de **Makefile** oluşturması
lazım. f5 tuşu ile oluşturduğu Makefile lar sonucu programı build edip
çalıştıracaktır.

### Windows için çalıştırma
İnternetten mingw yükleyip path'e mingw/bin dosyasını atmanız lazım.
Projeyi vscode'da açtıktan sonra Ctrl + Shift + B yapın.
Yukarıdaki Terminal yerinden **New Terminal** e tıklayın.
Açılan terminale **make** yazın. Workspace'de iki tane yeni dosya açılması lazım (*bin* ve *bin-int* dosyaları).
Bin dosyasını açın bin'in hemen altındaki dosyanın adını launch.json'daki
>"program": "${workspaceFolder}/bin/Debug-linux/Default/Default",

Debug-linux yazan yere o dosyanın yazın.

## Projenin adını değiştirme

Projenin adını değiştirmek istiyorsanız premake5.lua
dosyasında ve launch.json daki iki şeyi değiştirmeniz
gerekiyor. premake5.lua dosyasında Ctrl + H ile
find and replace yapıp Default kelimesini bulup
projenizin adıyla değiştirebilirsiniz. launch.json
dosyasında da aynı şeyi yaparsanız program
çalışmaya hazır demek.

Not: Adı Default olan dosyaların adını da değiştirmeyi
unutmayın!