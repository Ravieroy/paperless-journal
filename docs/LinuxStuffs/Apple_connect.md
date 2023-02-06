# Connecting iPad and iPhones to Linux
Links: [Opensource.com](https://opensource.com/article/21/8/libimobiledevice-iphone-linux), [maketecheasier.com](https://www.maketecheasier.com/easily-mount-your-iphone-as-an-external-drive-in-ubuntu/)

---

For iPhone and other iOS devices to be recognized on Ubuntu, you’ll need to install the `libimobiledevice` library first. This allows Ubuntu and other Linux operating systems to interact with these iOS devices.

```bash
sudo apt install usbmuxd libimobiledevice6 libimobiledevice-utils

```
Once `libimobiledevice` has installed, try to connect your iPhone. It should connect and should show your iOS file system. *You might not see all the folders though*. If that is the case, then you need to install `ifuse` 

```bash
sudo apt install ifuse
```

You can install the above-mentioned libraries in any [[Linux distros]] using their [[Package manager]]. 

If your iPhone file system doesn’t mount automatically when connected, you may need to pair your iPhone. Open a terminal and type:

```bash
idevicepair pair
```

If you want multiple connections between your iPhone and your Ubuntu installation. After pairing run the following code in your [[Terminal]]

```bash
usbmuxd -f -v
```

