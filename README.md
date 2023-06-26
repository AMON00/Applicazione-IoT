# Progetto-IoT
Implementazione di un applicazione IoT utilizzando l'esp32 come client per l'acquisizione dei dati e una macchina virtuale con installato Ubuntu 22.04 come broker Mqtt. Utilizzo di Node-Red per l'implementazione della dashboard ed inoltre i dati attraverso la dashboard vengono salvati su un database.

I componenti hardware utilizzati sono:
* ESP32-WROOM-32
* Sensore della temperatura e della pressione BMP280
* Sensore della luminosità BH1750
* Sensore RTC PCF8523


Altri componenti che sono stati utilizzati sono:
* Mosquitto come Mqtt broker
* Arduino per il codice caricaro sull'esp32
* Node-red per la creazione della dashboard
* Xampp per quanto riguarda la parte del salvataggio dei dati

## Installazione componenti software
### Mosquitto Broker
Aprire il terminale di Ubuntu e immetere le seguenti righe di comando per installare sul proprio dispositivo il Broker Mqtt Mosquitto
```
sudo apt update -y && sudo apt install mosquitto mosquitto-clients -y
sudo systemctl status mosquitto
sudo systemctl enable mosquitto
```
### Installazione Arduino
Scaricare dal seguente [link](https://support.arduino.cc/hc/en-us/articles/360019833020-Download-and-install-Arduino-IDE) l'ide di Arduino e dopo da terminale digitare le seguenti righe di comando:
```
cd /home/Scaricati
tar -xvf arduino-ide_2.1.0_Linux_64bit.tar.xz
sudo mv arduino-ide_2.1.0_Linux_64bit /opt/
sudo /opt/arduino-ide_2.1.0_Linux_64bit/install.sh
```
### Installazione Node-Red
Per installare Node-Red aprire il terminale e digitare le seguenti righe di comando:
```
sudo apt update
sudo apt install nodejs
node --version
npm --version
sudo npm install -g --unsafe-perm node-red
```
Una volta installato Node-Red per il suo avvito si utilizza:
```
node-red
```
### Installazione Xampp
Per installare Xampp aprire il terminale e digitare le seguenti righe di comando:
```
cd /home/Scaricati
sudo ./xampp-linux-x64-8.2.4-0-installer.run
```
Una volta installato per il suo avvio digitare il seguente comando da terminale:
```
sudo /opt/lampp/lampp start
```

  
  
