LXDE virtual desktop running in Docker container.

Use VNC Viewer to access the desktop with 'passw0rd' as the password. Don't forget to forward the 5900 port on your host (VirtualBox, VMW Workstation).

To start the container, simply type :
```
[prompt]> docker run -d -p 5900:5900 me My-Desktop besn0847/desktop-light:1.0
```

To change VNC password :
```
[prompt]> x11vnc -storepasswd $PASS /home/default/.x11vnc/passwd
```

Minimal desktop screenshot :

<img src="https://github.com/besn0847/desktop-light/raw/master/desktop-light.png" width=400/>

Software included in this container :

* All the software from desktop-mini:1.0 +
* firefox
* owncloud-client
* filezilla
* xpdf
* gimp
