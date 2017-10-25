# orange_pi_camera
## Setting up Orange Pi Camera on OPI lite

Install Armbian

First install modules for single use
```shell
sudo modprobe gc2035
sudo modprobe vfe_v4l2
```
For permenant usage add the following to 
* gc2035
* vfe_v4l2
```shell
sudo nano /etc/modules
```

Install FSWebCam
```shell
sudo apt install fswebcam
```

Take a Photo
```shell
fswebcam -f 50 -D 1 -r 640*480
```
