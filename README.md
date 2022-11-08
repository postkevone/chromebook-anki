# chromebook-anki
Install the latest version of Anki on arm64 Chromebooks (Tested on Lenovo Duet with Anki 2.1.54)


```
sudo apt install python3-pyqt5 python3-pyqt5.qtwebengine python3-pip
cd /usr
sudo git clone https://github.com/postkevone/chromebook-anki.git
pip install chromebook-anki/anki-2.1.47-cp38-abi3-manylinux2014_aarch64.whl
pip install chromebook-anki/aqt-2.1.47-py3-none-any.whl
pip install protobuf==3.20.*
pip install --upgrade anki
pip install --upgrade aqt
sudo apt install mpv
sudo mv chromebook-anki/anki.desktop /usr/share/applications/anki.desktop
sudo mv chromebook-anki/anki.png /usr/share/pixmaps/anki.png
sudo rm -r chromebook-anki
anki
```


To update Anki in the future just use


```
pip install --upgrade anki
pip install --upgrade aqt
```


# Credit


https://github.com/krmanik/anki-arm64
