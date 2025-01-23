### Huawei Wechselrichter per ESPHome anbinden

Verkabelung
- Verbinden Sie den ESP RX-Pin mit dem RX des RS485-Moduls
- Verbinden Sie den ESP TX-Pin mit dem TX des RS485-Moduls
- Verbinden Sie den A-Pin des RS485-Moduls mit dem freien Modbus-A-Pin am COM-Port Ihres Wechselrichters (Pin 1)
- Verbinden Sie den B-Pin des RS485-Moduls mit dem freien Modbus-B-Pin am COM-Port Ihres Wechselrichters (Pin 2)
- Wenn Sie ein abgeschirmtes Kabel verwenden, wird dringend empfohlen, die Abschirmung NUR AUF EINER SEITE an GND anzuschließen

Schauen Sie im Handbuch Ihres Wechselrichters nach, um den COM-Port zu finden. Die Pinnummern sind im Port selbst sichtbar.

#### Pinbelegung Stecker Wechselrichter
A+ - 1  
B-  - 3


| Anmerkung | Bild |
|----------|----------|
| Anschluss am Stecker des Wechselrichters | <img src="https://github.com/user-attachments/assets/852e601d-84c9-4ec7-9957-5182d5558eaa" width="280px">   | 
| Anschluss der Datenleitung am TTL-Adapter | <img src="https://github.com/user-attachments/assets/7e676fcf-7178-4bac-9573-4a939a976547" width="280px">   |
| Anschluss der Datenleitung am TTL Adapter zum ESP32 | <img src="https://github.com/user-attachments/assets/cc5942c7-cd3a-412c-b93a-5fc789122135" width="280px">   |
| Anschluss am ESP32 | <img src="https://github.com/user-attachments/assets/6f3fd278-b226-4355-ba96-ed46ca7e7192" width="280px">   |



Im Homeassistant -> ESPHome ein neues Gerät hinzufügen und folgende Einstelleungen hinterlegen:

config.yml
