# Default C++ Premake

## Projeyi çalıştırma

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
>Windows'da mingw yüklemeniz lazım.

İhtiyacınız olan aletleri aldığınıza göre şimdi ana projeyi vscode'da
açın. Ctrl + Shift + B yaparsanız premake'i çalıştıracaktır. Sonucunda
bir tane projenin altında, bir tane workspace de **Makefile** oluşturması
lazım. f5 tuşu ile oluşturduğu Makefile lar sonucu programı build edip
çalıştıracaktır.

## Projenin adını değiştirme

Projenin adını değiştirmek istiyorsanız premake5.lua
dosyasında ve launch.json daki iki şeyi değiştirmeniz
gerekiyor. premake5.lua dosyasında Ctrl + H ile
find and replace yapıp Default kelimesini bulup
projenizin adıyla değiştirebilirsiniz. Launc.json
dosyasında da aynı şeyi yaparsanız program
çalışmaya hazır demek.

Not: Adı Default olan dosyaların adını da değiştirmeyi
unutmayın!