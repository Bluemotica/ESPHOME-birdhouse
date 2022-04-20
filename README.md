# ESPHOME-birdhouse
A default ESPHOME configuration for use with my birdhouse with WIFI camera

This is based on the default ESPHOME software and you can find this at: https://esphome.io/guides/getting_started_hassio.html

It mainly use 3 integrations from ESPHOMe

1) the Camera module: https://esphome.io/components/esp32_camera.html?highlight=esp32%20cam
2) the Camera webserver module: https://esphome.io/components/esp32_camera_web_server.html?highlight=esp32%20cam
3) the Home-assistant integration: https://esphome.io/components/mqtt.html?highlight=mqtt#using-with-home-assistant

If you don't use Home-assistant, but you want to use MQTT services. you can enable this in the configuration at the #MQTT comments.
this uses the default MQTT integration.

---------

## Default setup:

*fast video for setup: https://github.com/Bluemotica/ESPHOME-birdhouse/blob/main/setup.mp4*

1. Download the birdhouse-camera.yaml code and open the ESPHOME dashboard.
2. pass the code into the editor: [alt text](https://github.com/Bluemotica/ESPHOME-birdhouse/blob/main/setup.gif)
3. open the file and alter the WIFI connection with your own user&password
4. Use or disable MQTT integration
5. Upload the code to the ESP32 chip.
6. Reboot the chip, and connect to it by ESHome dashboard or direct on the IP.


## usage

After setup you can look to the camera with any browser, just go to the IP of your camera or use the local DNS: http://ah_birdhouse.lan 
(if your router suport MDNS resolving). you will find an webspage with the switches and log:
[alt text](https://github.com/Bluemotica/ESPHOME-birdhouse/blob/main/webinterface.png)
* The  the videostream is on the configurated port (default 8081): http://ah_birdhouse.lan 
* The snapshot (default 8080) on: http://ah_birdhouse.lan:8080 

