# chromebook-anki
Install the latest version of Anki on arm64 Chromebooks (Tested on Lenovo Duet with Anki 2.1.54)


```
apt install python3-pyqt5 python3-pyqt5.qtwebengine python3-pip
```


Navigate to root/usr 


```
wget https://github.com/infinyte7/anki-arm64/releases/download/v0.0.1-ubuntu20.04/aqt-2.1.47-py3-none-any.whl
wget https://github.com/infinyte7/anki-arm64/releases/download/v0.0.1-ubuntu20.04/anki-2.1.47-cp38-abi3-manylinux2014_aarch64.whl
pip install anki-2.1.47-cp38-abi3-manylinux2014_aarch64.whl
pip install aqt-2.1.47-py3-none-any.whl
pip install protobuf==3.20.*
pip install --upgrade anki
pip install --upgrade aqt
apt install mpv
anki
```

In case the wget link stops working you can get the wheel files from the release section


To update Anki in the future just use


```
pip install --upgrade anki
pip install --upgrade aqt
```


# Credit


https://github.com/krmanik/anki-arm64
