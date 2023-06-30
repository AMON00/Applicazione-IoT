# Codice per l'ESP32
Prima di copiare il codice presente in questa parte della repository si devono scaricare la seguente libreria della scheda dell'esp32 copiandola nelle impostazioni delle preferenze sul software di Arduino ide e mettendo il seguente Url: https://espressif.github.io/arduino-esp32/package\esp32\index.json .

Una volta fatto ciò è possibile scegliere la scheda da utilizzare che ovviamente è ESP32-WROOM e scegliere anche la porta seriale di comunicazione per caricare lo sketch.
Succesivamente si devono installare dalle libreire di arduino le seguenti librerie:
* La libreria "Adafruit BMP280 library" per il sensore della temperatura e pressione
* La libreria "hp_BH1750" per il sensore della luminosità
* La libreria "RTClib" per quanto riguarda il sensore dell'ora e della data
* La libreria "PubSubClient" per la comunicazione del nostro client con il broker MQTT
*  La libreria "ArduinoJson" per il file json ricevuto da node-red attraverso il quale si estrae il timestamp per settare il PCF8523


Alcune librerie che non sono state citate qui, ma sono state usate sono già scaricate attraverso la libreria della scheda ESP32; una volta che si hanno tutte le librerie a disposizione si può copiare il codice presente in "Esp32_duetask.ino" e utilizzarlo per il proprio progetto.
