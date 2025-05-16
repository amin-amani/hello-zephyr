# hello-zephyr
This project forked from https://github.com/ShawnHymel/introduction-to-zephyr

### build and run Docker
```
docker build -t env-zephyr-espressif -f Dockerfile.espressif .
docker run --rm -v ./workspace:/workspace -it env-zephyr-espressif bash
```
### make application
```
cd workspace/apps/01_blink
west build -p always -b esp32s3_devkitc/esp32s3/procpu -- -DDTC_OVERLAY_FILE =boards/esp32s3_devkitc.overlay
```

https://youtu.be/mTJ_vKlMS_4?si=CIEpjYqRgMANhomg
