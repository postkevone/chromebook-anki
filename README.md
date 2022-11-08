# chromebook-anki
Install the latest version of Anki on arm64 Chromebooks (Tested on Lenovo Duet with Anki 2.1.54)


```
apt install python3-pyqt5 python3-pyqt5.qtwebengine python3-pip
cd /usr
git clone https://github.com/postkevone/chromebook-anki.git
unzip master.zip
pip install anki-2.1.47-cp38-abi3-manylinux2014_aarch64.whl
pip install aqt-2.1.47-py3-none-any.whl
pip install protobuf==3.20.*
pip install --upgrade anki
pip install --upgrade aqt
apt install mpv
mv anki.desktop /usr/share/applications/anki.desktop
mv anki.png /usr/share/pixmaps/anki.png
rm master.zip anki-2.1.47-cp38-abi3-manylinux2014_aarch64.whl aqt-2.1.47-py3-none-any.whl README.md
anki
```


To update Anki in the future just use


```
pip install --upgrade anki
pip install --upgrade aqt
```


# Credit


https://github.com/krmanik/anki-arm64
