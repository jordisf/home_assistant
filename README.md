# home_assistant

hassbian image -> sd
Config Wifi before starting raspberry ( didn't work ). Now running on eth cable

* apt-get update
* apt-get upgrade


Mosquitto MQTT Broker: https://www.youtube.com/watch?v=AsDHEDbyLfg
  * http://mosquitto.org/
  * http://mosquitto.org/man/mosquitto-conf-5.html

Install mosquitto
apt-get install mosquitto
apt-get install mosquitto-clients

Config:
vim /etc/mosquitto/mosquitto.conf

typical configs:
allow_anonymous false
password_file /etc/mosquitto/pwfile
listener 1883

Set user & password for a mosquitto user
mosquitto_passwd -c /etc/mosquitto/pwfile
( note: restart service after user & pwd creation & modification )

