# chromebook-anki
Install the latest version of Anki on arm64 Chromebooks (Tested on Lenovo Duet with Anki 2.1.54)


```
apt install python3-pyqt5 python3-pyqt5.qtwebengine python3-pip
```


Navigate to root/usr 


```
wget https://github.com/postkevone/chromebook-anki/blob/2883ca6e126f5f2b2ba1515784fcb4b11ba40546/anki-2.1.47-cp38-abi3-manylinux2014_aarch64.whl
wget https://github.com/postkevone/chromebook-anki/blob/2883ca6e126f5f2b2ba1515784fcb4b11ba40546/aqt-2.1.47-py3-none-any.whl
pip install anki-2.1.47-cp38-abi3-manylinux2014_aarch64.whl
pip install aqt-2.1.47-py3-none-any.whl
pip install protobuf==3.20.*
pip install --upgrade anki
pip install --upgrade aqt
apt install mpv
anki
```


To update Anki in the future just use


```
pip install --upgrade anki
pip install --upgrade aqt
```


# Credit


https://github.com/krmanik/anki-arm64
