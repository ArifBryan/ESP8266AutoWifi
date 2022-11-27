# ESP-Auto-Wifi

ESP Auto Connect Wifi without hardcode. Note that this code only works on ESP8266 architecture (includeing ESP01 and ESP12 series), for ESP32 go [here](https://github.com/aliffathoni/ESPAutoWifi).

## Dependencies

Make sure to download and install these library on your Arduino IDE before using ESPAutoWifi. You can download and install via link below since it doesn't included on Arduino Library Manager.

 - [ESPAsyncWebServer](https://github.com/me-no-dev/ESPAsyncWebServer)
 - [ESPAsyncTCP](https://github.com/me-no-dev/ESPAsyncTCP)
 - [Preferences](https://github.com/vshymanskyy/Preferences)


## Simple shortest code

You can use this code to use the main feature of this library.

```
  #include <ESPAutoWifi.h>

  ESPAutoWifi wf;

  void loop(){
    wf.autoConnect();
  }

  void loop(){

  }
```

It will automatically connect on last saved WiFi network, and if there is no saved network on your ESP then open your WiFi using other device(s) and connect to "ESP WiFi Portal" wifi, then type 192.168.4.1 on your browser to access the web portal.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE) file for details.
