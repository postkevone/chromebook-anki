# chromebook-anki
Install the latest version of Anki on arm64 Chromebooks (Tested on Lenovo Duet with Anki 2.1.54)


(sudo on pip is needed to install files on the default path)


```
sudo apt install python3-pyqt5 python3-pyqt5.qtwebengine python3-pip mpv fonts-noto-cjk
cd /usr
sudo git clone https://github.com/postkevone/chromebook-anki.git
sudo pip install chromebook-anki/anki-2.1.47-cp38-abi3-manylinux2014_aarch64.whl
sudo pip install chromebook-anki/aqt-2.1.47-py3-none-any.whl
sudo pip install protobuf==3.20.*
sudo pip install --upgrade anki
sudo pip install --upgrade aqt
sudo mv chromebook-anki/anki.desktop /usr/share/applications/anki.desktop
sudo mv chromebook-anki/anki.png /usr/share/pixmaps/anki.png
sudo rm -r chromebook-anki
```

In `anki.desktop` you can also set a custom folder
```
Exec=anki -b /mnt/chromeos/MyFiles/Anki2
```


To update Anki in the future just use


```
sudo pip install --upgrade anki
sudo pip install --upgrade aqt
```


# Credit


https://github.com/krmanik/anki-arm64
